close all
clear
clc
%
landareas = shaperead('landareas.shp','UseGeoCoords',true);
axesm ('mercator', 'Frame', 'on', 'Grid', 'on','origin',[0 0
0],'PLabelLocation',[-80:10:80],'PLabelMeridian',180,...
'ParallelLabel','on','FLonLim',[-180 180],'FLatLim',[-90
90]);
geoshow(landareas,'FaceColor',[1 1 .5],'EdgeColor',[.6 .6
.6]);
tissot;

