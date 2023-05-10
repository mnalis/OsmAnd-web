---
sidebar_position: 4
title:  Map during Navigation
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';
import AndroidStore from '@site/src/components/buttons/AndroidStore.mdx';
import AppleStore from '@site/src/components/buttons/AppleStore.mdx';
import LinksTelegram from '@site/src/components/_linksTelegram.mdx';
import LinksSocial from '@site/src/components/_linksSocialNetworks.mdx';
import Translate from '@site/src/components/Translate.js';
import InfoIncompleteArticle from '@site/src/components/_infoIncompleteArticle.mdx';
import ProFeature from '@site/src/components/buttons/ProFeature.mdx';
import InfoAndroidOnly from '@site/src/components/_infoAndroidOnly.mdx';

<InfoIncompleteArticle/>

## Overview

This article describes how the mapping behavior in the OsmAnd app changes during navigation. This includes [animated location changes](#animate-location-change), the display of [POIs along the route](#show-poi-along-the-route), the use of [screen alerts](#screen-alerts), the[appearance of the route line](#route-line-appearance) including color and width, and turn arrows. These features are closely related to the [route navigation settings](../navigation/route-navigation.md#settings).


## Map during navigation

Description of the change in map behavior during navigation.

<Tabs groupId="operating-systems">

<TabItem value="android" label="Android">

*<Translate android="true" ids="shared_string_menu,configure_profile,routing_settings_2"/>*  

| Parameter | Description | Note |
|:------------|:---------------|:---------------|
| "<Translate android="true" ids="choose_auto_follow_route"/>" |  The time before the map view is synchronized with the current position after moving.  |  Value: <br /> Never, 5 sec, 10 sec, 15 sec, 20 sec, 25 sec, 30 sec, 45 sec, 60 sec, 50 sec.|
| "<Translate android="true" ids="auto_zoom_map"/>"  |  Automatically scale the map according to your speed (as long as the map is in sync with your current position). | Value: <br /> *<Translate android="true" ids="auto_zoom_none"/>* - manually zoom. <br /> *<Translate android="true" ids="auto_zoom_farthest"/>* - zoom is 200m.<br /> *<Translate android="true" ids="auto_zoom_far"/>* - zoom is 100m. <br /> *<Translate android="true" ids="auto_zoom_close"/>* - zoom is 50m. |
| "<Translate android="true" ids="snap_to_road"/>"  |  The current position icon will be associated with the current navigation route.   | This option can be turned off, but then all road-related options, such as lane display, will also not be visible during navigation.   |
| "<Translate android="true" ids="approximate_bearing"/>"  |  Deriving the bearing from the navigation route being followed.    | The setting is visibled only if OsmAnd [Development plugin](../plugins/development.md) is enabled. <br /> This option can be turned on for case when movement direction map orientation ([Android Auto using](../navigation/auto-car.md#issues)) is flipped and juggles.   |

</TabItem>

<TabItem value="ios" label="iOS">

*<Translate ios="true" ids="shared_string_menu,shared_string_settings,application_profiles"/>*  

| Parameter | Description | Note |
|:------------|:---------------|:---------------|
| "<Translate ios="true" ids="choose_auto_follow_route"/>" |  The time before the map view is synchronized with the current position after moving.   |  Value: <br /> Never, 5 sec, 10 sec, 15 sec, 20 sec, 25 sec, 30 sec, 45 sec, 60 sec, 50 sec. |
| "<Translate ios="true" ids="auto_zoom_map"/>"  |  Automatically scale the map according to your speed (as long as the map is in sync with your current position).  | Value: <br />  *<Translate ios="true" ids="auto_zoom_none"/>* - manually zoom. <br /> *<Translate ios="true" ids="auto_zoom_farthest"/>* - zoom is 200m. <br /> *<Translate ios="true" ids="auto_zoom_far"/>* - zoom is 100m. <br /> *<Translate ios="true" ids="auto_zoom_close"/>* - zoom is 50m. |
| "<Translate ios="true" ids="snap_to_road"/>"  |  The current position icon will be associated with the current navigation route.  | This option can be turned off, but then all road-related options, such as lane display, will also not be visible during navigation.   |

</TabItem>

</Tabs>


## Animate location change

This setting provides a smooth animation of the "My location" point moving on the map during navigation. Note that the animation takes about 1 second, which creates a slight delay for the "My location" position to display on the map relative to your location.
For Android, this item named [Animate own position](#other) is located in the "Other" section of the General Settings menu.


## Show POI along the route


## Screen alerts

<Tabs groupId="operating-systems">

<TabItem value="android" label="Android">

*<Translate android="true" ids="shared_string_menu,configure_profile,routing_settings_2"/>*  

| Parameter | Description | Note |
|:------------|:---------------|:---------------|
| **<Translate android="true" ids="screen_alerts"/>** | Show or not show notifications on the screen as a widget. Alerts appear at the bottom left during navigation. | [Types of alert widgets](../widgets/nav-widgets.md#alert-widget)   |

</TabItem>

<TabItem value="ios" label="iOS">

*<Translate ios="true" ids="shared_string_menu,shared_string_settings,application_profiles,routing_settings_2"/>*  

| Parameter | Description | Note |
|:------------|:---------------|:---------------|
| **<Translate ios="true" ids="screen_alerts"/>** | Show or not show notifications on the screen as a widget.  | [Types of alert widgets](../widgets/nav-widgets.md#alert-widget)   |

</TabItem>

</Tabs>


## Route line appearance

This menu allows you to adjust the appearance of the route line to a variety of changes. These can be changes in elevation while driving, the next significant uphill or downhill, ice, unpaved roads, autobahns, and others. In the items on this menu, you can change all these parameters by color or choose the color and transparency of the line. In addition, you can change the line width and angle display on turns.  

:::note
<ProFeature/> Some parameters you can use only with <a href="https://osmand.net/docs/user/purchases/android#free-and-paid-features">OsmAnd Pro subscribtion</a>.
:::

<Tabs groupId="operating-systems">

<TabItem value="android" label="Android">

*<Translate android="true" ids="profile_type_user_string,shared_string_settings,configure_profile,routing_settings_2,customize_route_line"/>*  

![Navigation route Android](@site/static/img/navigation/route/RLApp.png)  

</TabItem>

<TabItem value="ios" label="iOS">  

*<Translate ios="true" ids="shared_string_menu,shared_string_settings,application_profiles,routing_settings_2,customize_route_line"/>*

![Navigation route Android](@site/static/img/navigation/route/RLApp_iOS.png)

</TabItem>

</Tabs>  


### Customize route line menu items


### Color

Select a route line's color by types.  

<Tabs groupId="operating-systems">

<TabItem value="android" label="Android">

|  |
|------------|
|&nbsp;*"<Translate android="true" id="map_widget_renderer"/>"* – Map style is used with default colors. You can see a full description of the colors by clicking here [Map style](../map/vector-maps.md#default-map-styles) |  
![map stule](@site/static/img/navigation/route/map_st_2.png) |
| &nbsp;*"Custom"* – It allows you to show the line in any preferred color and transparency. You can select different settings for the day map and separately for the night map. |  
![custom](@site/static/img/navigation/route/custom.png) |
| &nbsp;*"<Translate android="true" id="altitude"/>"* – It shows the height on the route point as **green**-**yellow**-**red** gradient. Where **green** represents lowest point of the route, **yellow** - median height points and **red** the highest points. If the route altitude difference is < 100 m, gradient is applied partially or not applied i.e. for a simple uphill route from 100 m to 150 m - the gradient will be **green**-**yellow**. Please note that the color doesn't represent the absolute height value.    |  
![Altitude](@site/static/img/navigation/route/Altitude_rl.png) |
|*<ProFeature/> &nbsp;"<Translate android="true" id="shared_string_slope"/>"* – The route line will be colored differently depending on the elevation profile of the route. [Slope](../plugins/contour-lines.md#slope-map)|
![Altitude](@site/static/img/navigation/route/Slope.png)  |
|*<ProFeature/> &nbsp;"<Translate android="true" id="routeInfo_roadClass_name"/>"* – Colour the route or the track line according to the road classification. [Road style](../map/vector-maps.md#road-style)|
![Altitude](@site/static/img/navigation/route/Roud_type.png)  |
|*<ProFeature/> &nbsp;"<Translate android="true" id="routeInfo_surface_name" />"* – Provides information about the physical surface of the road/footpath. [Surface](../map-legend/osmand.md#surface-smoothness)|
![Altitude](@site/static/img/navigation/route/Surface.png)  |
| *<ProFeature/> &nbsp;"<Translate android="true" id="routeInfo_smoothness_name"/>"* – Classification of maneuverability of roads/footpaths for wheeled vehicles, particularly with regard to surface regularity/flatness. [Smoothness](../map-legend/osmand.md#surface-smoothness)|
![Altitude](@site/static/img/navigation/route/Smoothness.png)  |
| *<ProFeature/> &nbsp;"<Translate android="true" id="routeInfo_winter_ice_road_name" />"* – Colouring the route or track line according to the winter road classification. [Winter and ice roads](../map/vector-maps.md#winter-and-ski)|
![Altitude](@site/static/img/navigation/route/Winter.png)  |
| *<ProFeature/> &nbsp;"<Translate android="true" id="routeInfo_tracktype_name" />"* – Colouring the route or track line by surface composition. Typically used when the road network is largely unpaved. [Surface firmness](../map-legend/osmand.md#surface-smoothness)| 
![Altitude](@site/static/img/navigation/route/firmness.png)  |
| *<ProFeature/> &nbsp;"Difficulty of horse trails"* – Render paths according to difficulty of horse trails.  |
![Altitude](@site/static/img/navigation/route/firmness.png)  |  

</TabItem>

<TabItem value="ios" label="iOS">  

|  |
|------------|
|&nbsp;*"<Translate android="true" id="map_widget_renderer"/>"* – Map style is used with default colors. You can see a full description of the colors by clicking here [Map style](../map/vector-maps.md#default-map-styles) |  
![map stule](@site/static/img/navigation/route/map_st_2.png) |
| &nbsp;*"Custom"* – It allows you to show the line in any preferred color and transparency. You can select different settings for the day map and separately for the night map. |  
![custom](@site/static/img/navigation/route/custom_ios.png) |
| &nbsp;*"<Translate android="true" id="altitude"/>"* –  It shows the height on the route point as **green**-**yellow**-**red** gradient. Where **green** represents lowest point of the route, **yellow* - median height points and **red** the highest points. If the route altitude difference is < 50 m, gradient is not applied i.e. for a simple uphill route from 100 m to 120 m. Please note that the color doesn't represent the absolute height value. |  
![Altitude](@site/static/img/navigation/route/Altitude_rl.png) |
|*<ProFeature/> &nbsp;"<Translate android="true" id="shared_string_slope"/>"* – The route line will be colored differently depending on the elevation profile of the route. [Slope](../plugins/contour-lines.md#slope-map)|
![Altitude](@site/static/img/navigation/route/Slope.png)  |
|*<ProFeature/> &nbsp;"<Translate android="true" id="routeInfo_roadClass_name"/>"* – Colour the route or the track line according to the road classification. [Road style](../map/vector-maps.md#road-style)|
![Altitude](@site/static/img/navigation/route/Roud_type.png)  |
|*<ProFeature/> &nbsp;"<Translate android="true" id="routeInfo_surface_name" />"* – Provides information about the physical surface of the road/footpath. [Surface](../map-legend/osmand.md#surface-smoothness)|
![Altitude](@site/static/img/navigation/route/Surface.png)  |
| *<ProFeature/> &nbsp;"<Translate android="true" id="routeInfo_smoothness_name"/>"* – Classification of maneuverability of roads/footpaths for wheeled vehicles, particularly with regard to surface regularity/flatness. [Smoothness](../map-legend/osmand.md#surface-smoothness)|
![Altitude](@site/static/img/navigation/route/Smoothness.png)  |
| *<ProFeature/> &nbsp;"<Translate android="true" id="routeInfo_winter_ice_road_name" />"* – Colouring the route or track line according to the winter road classification. [Winter and ice roads](../map/vector-maps.md#winter-and-ski)|
![Altitude](@site/static/img/navigation/route/Winter.png)  |
| *<ProFeature/> &nbsp;"<Translate android="true" id="routeInfo_tracktype_name" />"* – Colouring the route or track line by surface composition. Typically used when the road network is largely unpaved. [Surface firmness](../map-legend/osmand.md#surface-smoothness)| 
![Altitude](@site/static/img/navigation/route/firmness.png)  |
| *<ProFeature/> &nbsp;"Difficulty of horse trails"* – Render paths according to difficulty of horse trails.  |
![Altitude](@site/static/img/navigation/route/firmness.png)  | 

</TabItem>

</Tabs>  


### Width  

Select a route line's width.

<Tabs groupId="operating-systems">

<TabItem value="android" label="Android">

|  |
|------------|
|*"<Translate ios="true" id="map_settings_style"/>"* – It's used with default width. You can see a full description of the map style by clicking there [Map style](../map/vector-maps.md#default-map-styles)  |
![map style](@site/static/img/navigation/route/map_st.png)   ![map stule](@site/static/img/navigation/route/map_st_2.png) |
|*"Thin width / Medium width / Bold width"* – You can choose the width of the line according to the width of the road or highlight the line of the route on the map more strongly. |
![width](@site/static/img/navigation/route/width.png)   ![width](@site/static/img/navigation/route/width_med.png)|
|*"Custom"* – It allows you to show the line in some preferred width. Select the width using the slider.|
![custom](@site/static/img/navigation/route/custom_1.png)  ![custom](@site/static/img/navigation/route/custom_2.png)|  

</TabItem>

<TabItem value="ios" label="iOS">  

|  |
|------------|
|*"<Translate ios="true" id="map_settings_style"/>"* – It's used with default width. You can see a full description of the map style by clicking there [Map style](../map/vector-maps.md#default-map-styles)  |
![map style](@site/static/img/navigation/route/width_ms_ios.png)   ![map stule](@site/static/img/navigation/route/map_st_2.png) |
|*"Thin width / Medium width / Bold width"* – You can choose the width of the line according to the width of the road or highlight the line of the route on the map more strongly. |
![width](@site/static/img/navigation/route/width_ios.png)   ![width](@site/static/img/navigation/route/width_med.png)|
|*"Custom"* – It allows you to show the line in some preferred width. Select the width using the slider.|
![custom](@site/static/img/navigation/route/width_cus_ios.png)  ![custom](@site/static/img/navigation/route/custom_2.png)| 

</TabItem>

</Tabs>  

 
### Turn Arrows  

Select whether turn arrows are indicated on the route line or not. 

<Tabs groupId="operating-systems">

<TabItem value="android" label="Android">

|  |
|------------|
|![Altitude](@site/static/img/navigation/route/turn_arr.png) ![Altitude](@site/static/img/navigation/route/turn_arr_on_map_and.png)|
|![Altitude](@site/static/img/navigation/route/turn_arr_off_and.png) ![Altitude](@site/static/img/navigation/route/turn_arr_off_map_and.png)|

</TabItem>

<TabItem value="ios" label="iOS">  

|  |
|------------|
|![turn_arr_ios](@site/static/img/navigation/route/turn_arr_ios.png) ![turn_arr_ios_map](@site/static/img/navigation/route/turn_arr_ios_map.png)|
|![turn_arr_on_ios](@site/static/img/navigation/route/turn_arr_on_ios.png) ![turn_arr_ios_map](@site/static/img/navigation/route/turn_arr_ios_on_map.png) |

<!-- ![customise route line 1](@site/static/img/navigation/route/customise_route_line-1.png) -->

</TabItem>

</Tabs>  
