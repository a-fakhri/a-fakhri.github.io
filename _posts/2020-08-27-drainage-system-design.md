---
layout: post_no_comments
title: "Drainage System Design"
excerpt_separator:  <!--more-->
categories:
  - Projects
tags:
  - University Projects
  - Hydrotechnical Engineering

last_modified_at: 2017-03-09T13:01:27-05:00
---

### Project Overview
<div class="message">
This project was completed as part of the Municipal Engineering (CIVL 409) course at UBC.<br><br>

Our group was tasked with developing a Master Drainage Plan (MDP) for a new development in Deep Cove within
the District of North Vancouver. We were required to use the City of Surrey’s Design Criteria Manual as the basis of our design. As part of preparing the MDP, we needed to develop the conceptual layout to convey minor and major storm events, and identify the facilities and source control measures to protect the downstream aquatic habitat.<br><br>

The final report was submitted on April 5, 2019. A major portion of my contribution to the report (unedited since the date of submission) is displayed below. Click <a href="{{ site.url }}{{ site.baseurl }}/assets/pdfs/409 - Assignment 2 - Team 21 - Ali's Section only.pdf" download>here</a> to download the pdf version.
</div>
<!--more-->
---

### 3.4 Detention Pond
A detention pond was designed to safely discharge the 5-year storm and protect the downstream aquatic habitat. The pond was sized by modeling the proposed stormwater network in EPA SWMM and using the Kwantlen Park rainfall data from the Surrey Design Manual. The parameters of the pond were selected ensuring compliance with the guidelines listed in The City of Surrey Design Criteria Manual and the design criteria set by the client.

#### 3.4.1 Assumptions and Design Criteria
The source controls are assumed to be fully implemented and able to mitigate the 2-year storm; however,
they are assumed to not function under the 5-year storm. Section 5.2.1c. of the Surrey Design Manual
stipulates that the 5-year post-development flow rate needs to be controlled to 5-year pre-development
flow rate, assumed to be 7 L/s/ha. The development area is estimated to be 10.31 ha, hence the 5-year
post-development flow rate needs to be limited to 0.072 m<sup>3</sup>/s. A summary of the design criteria is shown
in Table 7.

*Table 7: Detention Pond Design Criteria*

| Design Criteria Description        | Criteria Value                                                                                  | Imposed by                     |
|------------------------------------|-------------------------------------------------------------------------------------------------|--------------------------------|
| Outlet Flow                        | 7 L/s/ha                                                                                        | Client                         |
| Pond Depth                         | 1.5 m                                                                                           | Client                         |
| Pond Side Slopes                   | 2:1                                                                                             | Client                         |
| Inlet Sewer to Pond Depth          | Crown of inlet manhole at or above the corresponding pond water level for the 1 in 5-year storm | Surrey Design Criteria 5.8.4.5 |
| Pond Inlet and Outlet Requirements | At least 0.1m above base of the pond                                                            | Surrey Design Criteria 5.8.4.4 |

The system was analyzed using the Kwantlen Park 5-year design storms with the following durations: 2-
hour, 6-hour, 12-hour, and 24-hour.


#### 3.4.2 EPA SWMM Model
The subcatchment areas were selected by considering the contour map of the study area and land zoning,
such that each area has a relatively constant slope and consistent zoning designation. The western
mountainous area was neglected since a swale was designed to direct that runoff into Gallant Creek. The
parks on the eastern side of the study area have also been neglected since they are assumed to either fully
absorb their runoff and/or direct it to the bay.

The setup of the stormwater network EPA SWMM model is shown in Figure 16. The parameter notation
used in SWMM is presented in Table 9. The values of the following subcatchment parameters are
summarized in Table 10: areas, overland flow lengths, widths, average surface slope, and percent of area
that is impervious. The overland flow length for each subcatchment was estimated by averaging several
possible overland flow paths measured in AutoCAD. The width of each subcatchment was found as a
ratio of its area to its overland flow length. The imperviousness percentages of areas were assigned
according to the Surrey Design Criteria, as shown in Table 8. Where a subcatchment contained more than
one land zoning, the percent imperviousness was assigned according to the proportion of the
subcatchment taken by each land zoning. The parameters used in developing the SWMM model along
with justifications are summarized in Table 11.

*Table 8: Imperviousness of Different Land Usages*

| Description of Area      | % Imperviousness |
|--------------------------|------------------|
| Commercial or Industrial | 90               |
| Residential              | 65               |
| Parks                    | 20               |
| Playgrounds              | 20               |
| Cemetery                 | 20               |
| Agricultural Land        | 20               |
| Institutional            | 80               |
| Passive Park             | 20               |



[![System Model Layout in EPA SWMM]({{ site.url }}{{ site.baseurl }}/assets/drainage_system_design_imgs/System_Model_Layout_in_EPA_SWMM.png)]({{ site.url }}{{ site.baseurl }}/assets/drainage_system_design_imgs/System_Model_Layout_in_EPA_SWMM.png)
*Figure 16: System Model Layout in EPA SWMM*

*Table 9: SWMM Parameter Notation*

| Parameter      | SWMM Notation |
|----------------|---------------|
| Subcatchment   | S             |
| Rain Gage      | R             |
| Pipes          | P             |
| Manholes       | MH            |
| Detention Pond | Pond1         |
| System Outlet  | Orif1         |

*Table 11: SWMM Design Parameter*

| Subcatchment ID | Area (ha) | Zoning                             | Overland flow length (m) | Width (m) | Slope (%) | % Impervious |
|-----------------|-----------|------------------------------------|--------------------------|-----------|-----------|--------------|
| S1              | 0.3714    | Residential                        | 50.0                     | 74.3      | 19.2      | 65.0         |
| S2              | 0.7973    | Residential                        | 96.2                     | 82.9      | 27.6      | 65.0         |
| S3              | 0.7990    | Residential                        | 91.3                     | 87.5      | 21.9      | 65.0         |
| S4              | 0.6896    | Residential                        | 51.5                     | 133.9     | 20.7      | 65.0         |
| S5              | 1.0069    | Residential                        | 105.0                    | 95.9      | 28.7      | 65.0         |
| S6              | 0.9012    | Residential and Commercial Village | 91.0                     | 99.0      | 24.9      | 75.0         |
| S7              | 0.4027    | Park and Commercial Village        | 112.0                    | 36.0      | 7.8       | 55.0         |
| S8              | 0.9058    | Residential                        | 49.5                     | 183.0     | 28.0      | 65.0         |
| S9              | 0.2973    | Residential                        | 35.6                     | 83.5      | 18.4      | 65.0         |
| S10             | 0.8940    | Residential                        | 91.7                     | 97.5      | 27.7      | 65.0         |
| S11             | 0.6522    | Residential                        | 60.9                     | 107.1     | 26.9      | 65.0         |
| S12             | 0.4665    | Residential                        | 44.0                     | 106.0     | 22.7      | 65.0         |
| S13             | 0.8057    | Residential                        | 84.3                     | 95.6      | 18.5      | 65.0         |
| S14             | 0.6598    | Park and Commercial Village        | 99.6                     | 66.2      | 13.9      | 60.0         |
| S15             | 0.6626    | Commercial Village                 | 90.0                     | 73.6      | 6.3       | 90.0         |

#### 3.4.3 Analysis and Results

The proposed stormwater network was analyzed in EPA SWMM by running the 2-hour, 6-hour, 12-hour,
and 24-hour duration 5-year design storms. The flow hydrographs at the outfall were then exported into
an Excel spreadsheet. These were then used as inflows into a pond with a trial size and a stepwise mass
balance at 5-minute intervals was then developed to estimate pond depths and outflows (evaluated using
the orifice equation). The shape of the pond and the orifice were selected to be a truncated square pyramid
and a square, respectively. The pond’s base dimensions and depth along with the orifice height were
iterated to minimize the pond size while meeting the imposed design criteria. The final dimensions of the
pond and orifice are summarized in Table 12. The maximum depth and maximum outflow obtained for
various durations of storm runs are summarized in Table 13. The storm with the 24-hour duration was
found to be most critical for selecting the pond and orifice parameters. Equations that were used to find
the optimal pond parameters are presented in Appendix B.

*Table 12: Pond and Orifice Final Parameters*

| Design Object | Parameter Description     | Parameter Value |
|---------------|---------------------------|-----------------|
| Pond          | Base Length and Width (m) | 50              |
|               | Top Length and Width (m)  | 56              |
|               | Height (m)                | 1.5             |
|               | Volume (m3)               | 4218            |
| Orifice       | Height (m)                | 0.15            |
|               | Area (m2)                 | 0.0225          |

*Table 13: Maximum Pond Depth and Outflow for Different Duration 5-Year Storms*

| 5-year Storm Duration | Max Pond Depth (m) | Max Outflow (m<sup>3</sup>/s) |
|-----------------------|--------------------|--------------------|
| 24hr                  | 1.439              | 0.071              |
| 12hr                  | 1.309              | 0.068              |
| 6hr                   | 1.033              | 0.060              |
| 2hr                   | 0.577              | 0.043              |
| Limit                 | 1.5                | 0.072              |

The orifice and pond were then added to the SWMM to verify the calculations. As seen in the time series
plots for the system under the 5-year 24-hour duration storm (Figure 17), the pond does not overflow, and
the pond’s discharge is limited to below the pre-development flow. The time series plots for other
durations of the 5-year storm are shown in Appendix C.


[![Time series plot]({{ site.url }}{{ site.baseurl }}/assets/drainage_system_design_imgs/Time Series Plot Under 5-Year 24-Hour Duration Storm.png)]({{ site.url }}{{ site.baseurl }}/assets/drainage_system_design_imgs/Time Series Plot Under 5-Year 24-Hour Duration Storm.png)
*Figure 17: Time Series Plot for Pond’s Hydraulic Parameters Under 5-Year 24-Hour Duration Storm*

The detention pond will be located in Panorama Park, slightly north of the last manhole. The location,
shape, and dimensions of the pond are shown in Figure 18.

<!-- [![Location, Shape and Dimensions of the Detention Pond]({{ site.url }}{{ site.baseurl }}/assets/drainage_system_design_imgs/pond location.png)]({{ site.url }}{{ site.baseurl }}/assets/drainage_system_design_imgs/pond location.png) [![Location, Shape and Dimensions of the Detention Pond]({{ site.url }}{{ site.baseurl }}/assets/drainage_system_design_imgs/pond dimensions.png)]({{ site.url }}{{ site.baseurl }}/assets/drainage_system_design_imgs/pond dimensions.png)
*Figure 18a: Location of the Detention Pond* -->

<img src="{{ site.url }}{{ site.baseurl }}/assets/drainage_system_design_imgs/pond location.png" style="width: 50%;"/> <img src="{{ site.url }}{{ site.baseurl }}/assets/drainage_system_design_imgs/pond dimensions.png" style="width: 50%;"/>

*Figure 18: Location, Shape and Dimensions of the Detention Pond*
