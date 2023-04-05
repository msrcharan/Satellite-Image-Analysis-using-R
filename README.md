# Satellite-Image-Analysis-using-R

<p> The project is designed to analyze the amount of deforestation, reduction in green vegetation, and the increase/decrease of water sources in the area. A satellite image of an area which can be collected from the open source websites such as zoom.earth or google maps could be used to analyze and report the amount of green vegetation and the water resources in that particular area. This application can be used to analyze the periodic changes in an area to take actions such as making stringent regulations to reduce deforestation, monitoring availability of water resources in order to take necessary measures in case of complete dry out. In this project, an image from zoom.earth(open-source) consisting of a large pixel sized csv file was generated, which was analyzed for monitoring the vegetation and water sources.
</p>

<hr>

## Methodology

<p>
First, the collected satellite image with dimensions (1858 x 895) was processed for the RGB values which lie in the range 0-255 for each channel. The rgb values which are the product of the dimensions (1,662,910) are generated and stored in a csv file whose sizes go up to 18MB. The data generated by the JPEG package in R language contains null values which were substituted with 1. This data is then used to find the highest intensity channel out of R, G and B. If the value of the green channel is higher than other channels, the value is added to the counter. This value is then divided by the total number pixels, to get the green vegetation index. These numbers are collected and stored in a csv file as periodic records for further assessment.
</p>

