This project visualizes the process of estimating Pi using the Monte Carlo method, using the Cora Z7-07S and a Pmod VGA. With the Pmod VGA plugged into Pmod connectors JA and JB, and the VGA port connected to a monitor, a 640x480 screen will be shown. Points are randomly generated and placed within a square on the screen at a selectable rate (see the table below). BTN0 resets the demonstration and BTN1 is used to iterate through the point generation rates.

LED1	LED0	Sample Rate
Off	Off	152.59 Hz
Off	On	610.35 Hz
On	Off	2.441 kHz
On	On	9.765 kHz
In order to use this demo, a Pmod VGA, a Cora Z7-07S, a VGA Monitor, and a VGA cable are required. For the Cora Z7-10 version of this project, see this repo.

For a full write up of this demo, see the Hackster Project (FIXME).

WARNING!!! This project is only supported in the 2017.4 version of Vivado.

In order to program the project onto an FPGA:

Download the most recent release ZIP archive (not the source ZIP) from the repo's releases page.

Extract and open the downloaded ZIP. Double click on "Cora-Z7-07S-Pi-Estimator-VGA.xpr". This will launch an archived version of the project, in which a bitstream has already been generated.

Open the Vivado Hardware Manager, select "Open Target", and find the target board.

Program top.bit, found in the Cora-Z7-07S-Pi-Estimator-VGA.runs/impl_1/ subdirectory of the extracted archive, onto the target.

For more information on how this project is version controlled, see the digilent-vivado-scripts repo, which contains several Python and TCL scripts for maintaining a Vivado project on Github.