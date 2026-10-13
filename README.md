# Cain Tipton — Project Portfolio

📧 caintipton2023@gmail.com &nbsp;|&nbsp;

---

## Table of Contents

- [Raze Defence — Real-Time Drone Detection System](#raze-defence--real-time-drone-detection-system)
- [ROB — AlohaMini2 + XLeRobot-Pro Manipulation Platform](#rob--alohamini2--xlerobot-pro-manipulation-platform)
- [AUV Object Detection & Mapping](#auv-object-detection--mapping)
- [Weather Hazard Tracking Software](#weather-hazard-tracking-software)
- [BS Movie Review Website](#bs-movie-review-website)
- [Custom Online Grocery Store](#custom-online-grocery-store)
- [Drone Delivery Network Optimization](#drone-delivery-network-optimization)
- [Animal Overpass Proposal](#animal-overpass-proposal)
- [Historic Fire Analysis of the Okanagan Valley](#historic-fire-analysis-of-the-okanagan-valley)

---
## Raze Defence — Real-Time Drone Detection System

Joined Raze Defence as an ML & Computer Vision Co-op on the company's first day of operation, serving as the primary ML and software lead at an early-stage startup. Over four months, I took ambiguous, fast-changing requirements and shipped solutions across model development, data infrastructure, and software, from an early internal developer GUI to a full-stack operator web app for the real-time detection system.

<table>
  <tr>
    <td><img src="images/Raze_Defence/raze_1.jpg" alt="Earlier 360-degree prototype" width="350"/></td>
    <td><img src="images/Raze_Defence/raze_2.gif" alt="Most recent product version" width="350"/></td>
  </tr>
  <tr>
    <td align="center"><em>An earlier prototype aimed at a 360° target view</em></td>
    <td align="center"><em>Most recent product version prior to departure</em></td>
  </tr>
</table>

### Skills Demonstrated

- ML and software leadership at an early-stage startup, translating ambiguous requirements into shipped solutions
- Object detection and real-time inference (PyTorch, RF-DETR, OpenCV)
- Data infrastructure and tooling: AWS S3 management, a SAM2-based auto-annotator, and a custom data auditing script
- Edge deployment on NVIDIA Jetson Orin NX, validated against FLIR camera and RTX 4080 hardware
- Full-stack development, building an operator web application on top of production detection/tracking logic

---

## ROB — AlohaMini2 + XLeRobot-Pro Manipulation Platform

A long-term personal project fusing AlohaMini2 and XLeRobot-Pro into an at-home manipulation robot I'm calling "ROB." I upgraded the compute and perception stack, built the full hardware myself, and am now collecting data to train policies for real household tasks. The goal is to learn the hardware fundamentals of robotics while applying AI to real-world manipulation.

<table>
  <tr>
    <td><img src="images/ROB/rob_1.png" alt="AlohaMini2 base platform" width="300"/></td>
    <td><img src="images/ROB/rob_2.jpg" alt="XLeRobot-Pro compute and perception" width="300"/></td>
    <td><img src="images/ROB/rob_3.gif" alt="Combined ROB platform" width="300"/></td>
  </tr>
  <tr>
    <td align="center"><em>AlohaMini2 base</em></td>
    <td align="center"><em>XLeRobot-Pro compute/perception</em></td>
    <td align="center"><em>Combined into ROB</em></td>
  </tr>
</table>

![RTAB-Map world model output](images/ROB/rob_4.png)
*Collecting teleoperated demonstrations and RGB-D data to build a world model of my home using RTAB-Map*

![Hardware debugging](images/ROB/rob_5.jpeg)
*Fixing a broken wire snapped during assembly, part of the hands-on hardware reality of building a robot from scratch*

### Skills Demonstrated

- End-to-end hardware build: assembly, wiring, and electrical troubleshooting on a physical robot
- Compute and perception upgrade integrating an NVIDIA Jetson Orin Nano, Intel RealSense D436, and wide-angle cameras
- RGB-D visual SLAM and mapping (RTAB-Map) to build a real-time world model of the environment
- Teleoperated demonstration data collection in preparation for imitation learning, reinforcement learning, and VLA-model policy training
- ROS2 and PyTorch development on embedded Linux (Ubuntu)

---

## AUV Object Detection & Mapping

### Object Detection Update

Assisted in the development of the `detmodel_test.py` script to improve evaluation of our `gate_onnx` model. The goal is to navigate the AUV through a gate during competition, but the model previously struggled with reliable detection. The updated script focused on removing post-processing bugs and improving detection accuracy.

| Before | After |
|--------|-------|
| ![Predicted mask before fix](images/Marine_Robotics/robotics_1.png) | ![Ground truth after fix](images/Marine_Robotics/robotics_2.png) |

### Mapping Update

Researched and evaluated visual SLAM architectures to incorporate mapping into the AUV. After analysis, determined that combining the existing PCL-based detection pipeline with SLAM-based models was the best approach for competition requirements.

<table>
  <tr>
    <td><img src="images/Marine_Robotics/robotics_3.png" alt="Point cloud mapping in pool" width="400"/></td>
    <td><img src="images/Marine_Robotics/robotics_4.png" alt="Live object detection in pool" width="400"/></td>
  </tr>
  <tr>
    <td align="center"><em>Point cloud mapping output during pool testing</em></td>
    <td align="center"><em>Live object detection during pool testing</em></td>
  </tr>
</table>

### Skills Demonstrated

- Computer vision and object detection model evaluation and optimization
- Automated testing frameworks for model validation and iterative debugging
- Robotics perception pipeline development (ONNX Runtime, PCL, SLAM)
- ROS2 integration and sensor pipeline debugging

---

## Weather Hazard Tracking Software

A full-stack geospatial application built for Environment Canada's Coastal Prediction Center to store, visualize, and query extreme weather events. The system allows forecasters to be aware of an event's lasting effects and assess compounded risks across western Canada.

Users can create a hazard polygon by entering event details, plotting boundary points on an interactive map, and saving the record to the server for persistent access.

![Weather Hazard Tracker interface](images/Hazard_Tracker/hazard_1.png)

<table>
  <tr>
    <td><img src="images/Hazard_Tracker/hazard_2.png" alt="Enter hazard info" width="250"/></td>
    <td><img src="images/Hazard_Tracker/hazard_3.png" alt="Edit hazard pane" width="250"/></td>
    <td><img src="images/Hazard_Tracker/hazard_4.png" alt="Create hazard pane" width="250"/></td>
  </tr>
  <tr>
    <td align="center"><em>1. Enter event info</em></td>
    <td align="center"><em>2. Plot on map & edit</em></td>
    <td align="center"><em>3. Save to server</em></td>
  </tr>
</table>

### Skills Demonstrated

- Full-stack development: React frontend with interactive geospatial mapping, Node.js backend with RESTful API architecture
- Database design for storing and retrieving spatial event data
- Translating operational user requirements into a production-deployed application

---

## BS Movie Review Website

A full-stack movie review platform developed as a term-long Software Engineering course project. Built with a FastAPI backend and Next.js frontend, with a focus on clean architecture, automated testing, and containerized deployment.

![Movie review website landing page](images/Movie_Review/movie_1.png)

<table>
  <tr>
    <td><img src="images/Movie_Review/movie_2.png" alt="Backend architecture" width="400"/></td>
    <td><img src="images/Movie_Review/movie_3.png" alt="Unit and integration tests" width="400"/></td>
  </tr>
  <tr>
    <td align="center"><em>Backend project architecture</em></td>
    <td align="center"><em>Unit and integration tests for the search algorithm</em></td>
  </tr>
</table>

### Skills Demonstrated

- RESTful API implementation and database design
- Writing clean, modular code with comprehensive documentation
- Automated testing with 93% coverage via Pytest
- Docker containerization for cross-platform deployment

---

## Custom Online Grocery Store

A full-featured e-commerce platform developed for a Database Systems course, modelled after a standard online grocery experience. Built with a Node.js/Express backend and MySQL database, with full ACID-compliant transaction management.

![Grocery store landing page](images/Grocery_Store/store_1.png)

<table>
  <tr>
    <td><img src="images/Grocery_Store/store_2.png" alt="Dockerized project" width="400"/></td>
    <td><img src="images/Grocery_Store/store_3.png" alt="Project architecture" width="300"/></td>
  </tr>
  <tr>
    <td align="center"><em>Application containerized with Docker</em></td>
    <td align="center"><em>Project architecture</em></td>
  </tr>
</table>

**Key features:** user login/signup, shopping cart, admin tools, secure authentication, dynamic product catalog.

### Skills Demonstrated

- MySQL database design with ACID-compliant transaction management
- Secure user authentication and session handling
- Docker containerization and Git version control workflows

---

## Drone Delivery Network Optimization

A comparative spatial analysis examining how delivery mode fundamentally alters optimal hub placement, conducted across two scenarios in San Francisco.

**Ground-based scenario:** Used ArcGIS Pro's Location-Allocation solver with population-weighted census demand data to identify 11 optimal hub locations capturing 70% market share, competing against existing store locations.

**Drone scenario:** Built a multi-criteria cost surface raster combining LiDAR-derived building heights, FAA airspace altitude ceilings, terrain elevation, slope, and power line constraints — weighted and reclassified to a 0–100 cost scale with hard no-fly masks applied post-analysis for FAA 0ft ceiling cells and NPS-restricted zones. Currently applying Least-Cost Path analysis with integrated census income and population density data to identify hub placements that maximize population coverage while minimizing flight cost across the constraint surface.
<img src="images/drone_project/drone_3.png" alt="Weighted sum cost-layer" width="400"/>
 <em>Weighted sum cost-layer</em>
<table>
  <tr>
    <td><img src="images/drone_project/drone_1.png" alt="Raw candidate location data" width="400"/></td>
    <td><img src="images/drone_project/drone_2.png" alt="Optimized hub locations" width="400"/></td>
    
  </tr>
  <tr>
    <td align="center"><em>Raw candidate and competitor store data</em></td>
    <td align="center"><em>Optimized hub placements — 70% market share result</em></td>
  </tr>
</table>

### Skills Demonstrated

- Location-Allocation optimization (Maximize Coverage, Minimize Impedance, Maximize Market Share)
- Multi-criteria raster analysis with weighted cost surfaces
- FAA airspace constraint integration as polygon barriers
- Least-Cost Path routing and cost-based spatial search

---

## Animal Overpass Proposal

A spatial analysis identifying optimal locations for a wildlife overpass along Highway 16 in Jasper, Alberta. The goal was to determine routes that facilitate safe animal movement while minimizing conflict with human infrastructure.

Ten input rasters, including land cover, elevation, and human proximity, were reclassified to a common 1–100 resistance scale and combined into a composite surface. Least-Cost Path analysis was then applied using designated habitat patch data to identify optimal crossing corridors.

<table>
  <tr>
    <td><img src="images/Overpass_Proposal/overpass_2.png" alt="Resistance surface model" width="350"/></td>
    <td><img src="images/Overpass_Proposal/overpass_1.png" alt="Final overpass proposal map" width="400"/></td>
  </tr>
  <tr>
    <td align="center"><em>Resistance surface model used for LCP analysis</em></td>
    <td align="center"><em>Final proposed overpass locations along Highway 16</em></td>
  </tr>
</table>

### Skills Demonstrated

- Multi-criteria evaluation and least-cost path algorithms
- Cost surface construction through rasterization and reclassification
- Large-scale spatial data transformation and processing

---

## Historic Fire Analysis of the Okanagan Valley

A spatial pattern analysis of forest fires in the Okanagan region between 2008 and 2018, comparing human-caused versus lightning-caused ignitions using a range of GIS statistical techniques.

Human-caused fires showed wider spatial clustering than lightning-caused fires, with distinct hotspot patterns and significant positive spatial autocorrelation in lightning fire sizes.

<table>
  <tr>
    <td><img src="images/Fire_Analysis/fire_1.png" alt="Raw fire distribution data" width="280"/></td>
    <td><img src="images/Fire_Analysis/fire_2.png" alt="Kernel density hotspot map" width="280"/></td>
    <td><img src="images/Fire_Analysis/fire_3.png" alt="Ripley's K function chart" width="350"/></td>
  </tr>
  <tr>
    <td align="center"><em>Raw fire distribution (2008–2018)</em></td>
    <td align="center"><em>Kernel density hotspot map</em></td>
    <td align="center"><em>Ripley's K function — spatial clustering analysis</em></td>
  </tr>
</table>

**Methods:** mean center calculations (weighted and unweighted by fire size), Ripley's K function for spatial clustering, kernel density estimation for hotspot identification, and Moran's Index for global and local spatial autocorrelation.

### Skills Demonstrated

- Point pattern analysis using Ripley's K function
- Kernel density estimation for hotspot identification
- Moran's Index for spatial autocorrelation
- Comparative spatial analysis of categorical data

---

*For questions or to connect, reach out at caintipton2023@gmail.com*
