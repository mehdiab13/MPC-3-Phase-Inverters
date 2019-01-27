# MPC for 3-Phase Inverters:
This repository contains the codes for control a three-phase inverter with output *LC* filter using **Model Predictive Control (MPC)**. The controller uses a discrete-time model of the system to predict the behavior of the output voltage for all possible switching states generated by the inverter. Then, a cost function is used as a criterion for selecting the switching state that will be applied during the next sampling interval. The simulations for MPC with only one-prediction step are presented under linear and nonlinear loads using `MATLAB/Simulink` tools. 

# Usage: 
- For Linear loads (i.e., Resistive), type in the Command window, for instance:
```
>> clear all, clc, Ts = 30e-6; Vref = 200; Cfilter = 40e-6; Lfilter = 2.5e-3; Vdc = 500; Res = 100; 
```
Then, run the Simulink model (i.e., **MPC_3Phase_Inverter.slx**)

- For Non-Linear loads (i.e., diode-bridge rectifier), type in the Command window, for instance:
```
 >> clear all, clc, Rnload = 100; Cnload = 500e-6; Ts = 30e-6; Lfilter= 4.0e-3; Cfilter = 45e-6; Vdc = 520; Vref = 250;
```
Then again, run the Simulink model. Do not forget to uncomment and connect the Non-Linear load ;-)

## Requirement:
This model was updated to be compatible with `Matlab R2018a` and the most recent versions.

## Citations:
**Eventually**, if you use the codes or relevant to your academic work, please cite one of the relevant articles :-), 

1. @inproceedings{mohamed2013three,<br/>
  title={[Three-phase inverter with output LC filter using predictive control for UPS applications](https://www.researchgate.net/profile/Ihab_S_Mohamed/publication/261151989_Three-phase_inverter_with_output_LC_filter_using_predictive_control_for_UPS_applications/links/5560bfcd08ae9963a119f91c/Three-phase-inverter-with-output-LC-filter-using-predictive-control-for-UPS-applications.pdf)},<br/>
  author={Mohamed, Ihab S and Zaid, Sherif A and Elsayed, Hany M and Abu-Elyazeed, MF},<br/>
  booktitle={Control, Decision and Information Technologies (CoDIT), 2013 International Conference on},<br/>
  pages={489--494},<br/>
  year={2013},<br/>
  organization={IEEE}<br/>
}<br/>

2. @article{mohamed2016implementation,<br/>
  title={[Implementation of model predictive control for three-phase inverter with output LC filter on eZdsp F28335 Kit using HIL simulation](https://www.researchgate.net/profile/Ihab_S_Mohamed/publication/303864370_Implementation_of_model_predictive_control_for_three-phase_inverter_with_output_LC_filter_on_eZdsp_F28335_Kit_using_HIL_simulation/links/57d2fe5608ae0c0081e26d67.pdf)},<br/>
  author={Mohamed, Ihab S and Zaid, Sherif A and Abu-Elyazeed, MF and Elsayed, Hany M},<br/>
  journal={International Journal of Modelling, Identification and Control},<br/>
  volume={25},<br/>
  number={4},<br/>
  pages={301--312},<br/>
  year={2016},<br/>
  publisher={Inderscience Publishers (IEL)}<br/>
}<br/>

3. @inproceedings{mohamed2013classical,<br/>
  title={[Classical methods and model predictive control of three-phase inverter with output LC filter for UPS applications](https://www.researchgate.net/profile/Ihab_S_Mohamed/publication/261152214_Classical_methods_and_model_predictive_control_of_three-phase_inverter_with_output_LC_filter_for_UPS_applications/links/5911d14e4585152e1989898a/Classical-methods-and-model-predictive-control-of-three-phase-inverter-with-output-LC-filter-for-UPS-applications.pdf)},<br/>
  author={Mohamed, Ihab S and Zaid, Sherif A and Abu-Elyazeed, MF and Elsayed, Hany M},<br/>
  booktitle={Control, Decision and Information Technologies (CoDIT), 2013 International Conference on},<br/>
  pages={483--488},<br/>
  year={2013},<br/>
  organization={IEEE}<br/>
}<br/>

4. @article{mohamed2015improved,<br/>
  title={[Improved model predictive control for three-phase inverter with output LC filter](https://s3.amazonaws.com/academia.edu.documents/43736557/Improved_model_predictive_control_for_th20160314-8606-1melg63.pdf?AWSAccessKeyId=AKIAIWOWYYGZ2Y53UL3A&Expires=1548624872&Signature=HPNaAnLJN577WoZOnhOA%2Bf0HAxM%3D&response-content-disposition=inline%3B%20filename%3DImproved_model_predictive_control_for_th.pdf)},<br/>
  author={Mohamed, Ihab S and Zaid, Sherif A and Abu-Elyazeed, MF and Elsayed, Hany M},<br/>
  journal={International Journal of Modelling, Identification and Control},<br/>
  volume={23},<br/>
  number={4},<br/>
  pages={371--379},<br/>
  year={2015},<br/>
  publisher={Inderscience Publishers (IEL)}<br/>
}<br/>


> For further information or codes of other articles (e.g., HIL implementation), please feel free to conatct me.
- **Ihab S. Mohamed**, INRIA Sophia Antipolis - Méditerranée, France, ihab.s.mohamed@gmail.com
