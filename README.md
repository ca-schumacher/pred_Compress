# Predictive maintenance of a first stage compressor

**August 2019**

**Project Description:**

We will use this dataset to analyse and predict the time the compressor should be maintained. For this we will focus on the lubrication system, the dry gas seal system, the condition monitoring system. 

**Data Description:**

The data has been retrieved through the **The Open Industrial Data Project**, the world's first live industrial data stream (https://openindustrialdata.com/). The dataset includes time series data, maintenance history, and Process & Instrumentation Diagrams (P&IDs). It can be accessed by using the Cognite Data Fusion API and SDK's.

## Description of the Unit
The data set represents the first of four stages for compression of natural gas on the Valhall PH platform. The purpose of the gas train is to compress and treat the gas to meet the required export pressure and specification, with a total capacity of 4,06 MSm3/d (143 MMscf/d).

The first stage compressor (23-KA-9101) is an electrically-driven, fixed-speed centrifugal compressor which receives gas from the separators at approximately 3 barg pressure. Before reaching the compressor, the gas is cooled in the first stage suction cooler (23-HA-9103), which is a shell-and-tube heat exchanger. The cooled gas flows into the first stage suction scrubber (23-VG-9101), which removes liquid droplets before the gas enters the compressor. The gas is compressed to approximately 12 barg and flows through a pair of discharge coolers (23-HA-9114/9115) before entering the second stage of compression.

Further info, especially about the involved components and their piping and instrumentation diagrams (P&ID) can be found in the appendix of this master thesis:
Enerstvedt, Å. (2010). VRD plant performance testing project (Master's thesis, University of Stavanger, Norway). https://uis.brage.unit.no/uis-xmlui/bitstream/handle/11250/182790/Enerstvetdt,%20%C3%85sbj%C3%B8rn.pdf?sequence=1 

### Control
Automatic control of the first stage compressor and associated process equipment is achieved by the following control loops:

The temperature at the suction cooler outlet is controlled by regulating the amount of cooling medium flowing through the shell side of the suction cooler.
The level in the first stage suction scrubber is controlled by regulating the amount of liquid flowing out of the scrubber. Excess liquids are sent back to the 2nd stage separator.
The pressure in the first stage separator is controlled by regulating the suction throttle valve (STV) upstream of the first stage suction scrubber, which controls the amount of gas sent to the compressor.
Anti-surge protection is achieved by recycling gas from downstream the discharge coolers back to the inlet. The amount of gas to be recycled is controlled by regulating the anti-surge valve (ASV). Since the recycle line is connected just upstream of the STV, the pressure. 

### Utility Systems
The following utility systems are also included in the data set:

The lubrication system for the first stage compressor. The system is comprised of pumps, coolers, filters, heating elements, and associated monitoring equipment, the purpose of which is to reduce friction and mechanical wear and to prevent overheating and corrosion in the compressor internals.
The dry gas seal system (DGS), the purpose of which is to prevent the process gas inside the compressor from escaping to the atmosphere.
The condition monitoring system (CMS), which monitors temperatures and vibrations in the motor, gearbox and compressor.

Source: https://openindustrialdata.com/data
