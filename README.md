# My-Jupyter-Notebook-on-IBM-Watson-Studio
JONATHAN NORIEGA 
![image](https://user-images.githubusercontent.com/126974834/229954422-c8d8c72e-d4a5-4d89-9859-1ce60066122c.png)
import geocoder # import geocoder

# initialize your variable to None
lat_lng_coords = None

# loop until you get the coordinates
while(lat_lng_coords is None):
  g = geocoder.google('{}, Toronto, Ontario'.format(postal_code))
  lat_lng_coords = g.latlng

latitude = lat_lng_coords[0]
longitude = lat_lng_coords[1]

