# FlexiTAC 


FlexiTAC is a Bayesian Flow Network developed for structure-based PROTAC linker design. It offers highly efficient sampling and accurate structure generation capabilities, and utilizes a posterior gradient guidance method to control linker flexibility.

[FlexiTAC enables controllable PROTAC linker generation across diverse structural settings using a Bayesian flow network with posterior guidance](https://www.biorxiv.org/content/10.64898/2026.08.26.747172v1)




# FlexiTAC UI

FlexiTAC UI is a lightweight interface built upon FlexiTAC for users to conveniently design PROTAC linkers. It supports local deployment on Mac and Linux.
See FlexiTAC_UI.mov for the demonstration.


# FlexiTAC interface
Enabling Programmable PROTAC linker design via FlexiTAC

```python

from interface import FlexiTAC

linker_size = FlexiTAC.size_prediction_module("FlexiTAC/interface/example_outputs/fragments.sdf")
anchors = FlexiTAC.anchor_prediction_module("FlexiTAC/interface/example_outputs/fragments.sdf")

result = FlexiTAC.generate("FlexiTAC/interface/example_outputs/fragments.sdf",
                           output_dir = "example",linker_size = linker_size,anchors = anchors)

```




