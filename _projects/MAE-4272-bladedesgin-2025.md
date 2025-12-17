---
layout: project
title: MAE 4272 Blade Design 
description: CAD, Fluid Mechanics, and Testing Project
technologies: [Fusion 360, MATLAB]
image: /assets/images/singleblade.png
---

For MAE 4272, our project focused on designing, fabricating, and testing a small-scale wind turbine blade optimized to maximize power output in a wind tunnel environment. The blade was designed to operate optimally at 1200 RPM under prescribed geometric, material, and operational constraints, including a maximum radius of 6 inches, maximum chord length of 2 inches, and a hard limit of 2000 RPM. Using Betz-limit blade element theory, we developed an optimized blade geometry and compared its theoretical power output to experimental performance obtained through wind tunnel testing.

![Final blade designs]({{ "/assets/images/bladedesign.png" | relative_url }}){: .inline-image-r style="width: 200px"}

The design process relied on blade element momentum theory under idealized assumptions, including operation at the Betz limit, no wake rotation, and isentropic material behavior. A MATLAB-based optimization model was developed to compute chord, pitch, and twist distributions along the blade radius. A NACA 6412 airfoil was selected to model our blade after for its high lift-to-drag ratio and suitability for low-speed conditions. Structural integrity was verified analytically by integrating lift-induced moments along the blade span and calculating bending stress, which remained well below allowable limits. These checks ensured the blade could safely withstand wind tunnel forces prior to testing.

Experimental validation was conducted in a controlled wind tunnel using fan frequencies from 6–10 Hz. At each wind speed, torque was incrementally applied via a torque brake until stall, then reduced to capture hysteresis effects. Data were collected using a LabVIEW-controlled DAQ system and post-processed to generate power curves at each operating condition. Experimental power output was calculated from measured torque and rotational speed and compared against theoretical predictions. While the blade met all structural and geometric constraints and operated safely, experimental performance fell significantly below theoretical expectations, with an average power output of 0.048 W compared to a predicted 1.528 W.

These are the power curves that we generated:

![Photo of power curve results]({{ "/assets/images/powercurve.png" | relative_url }}){: .inline-image-l}

This discrepancy highlights unmodeled aerodynamic and mechanical losses, including friction, non-ideal flow effects, and power transmission inefficiencies. Despite this gap, the project successfully validated the structural design and experimental methodology, providing a strong foundation for future iterations. Key improvements include incorporating non-ideal induction factors, optimizing for both power and torque, and increasing experimental resolution.  

My primary contributions included defining and calculating the design constraints, performing structural analysis, leading the experimental testing of the blade in the wind tunnel, and analyzing power curve data.


