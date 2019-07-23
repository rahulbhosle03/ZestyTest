## ZestyTest

## Setup  
    - Download repository
    - Add 'app' folder to same level as docker compose file.
    - In Terminal run docker-compose up

## API  
- Display, Display Plus

      Endpoint: 
        - localhost:4342/api/image/
      
      Arguments:
        - geoid(required) - ID
        - overlayParcel(optional) - 'true'
        - overlayBuilding(optional) - 'true'
  
      Description: 
        - This endpoint returns a binary image if only id is passed. If overlay arguments are passed it 
          returns an image overlay of the overlay options selected and a raster image.  

- Statistics

      Endpoint: 
       - localhost:4342/api/statistics/
      
      Arguments:
       - geoid(required) - ID
       - buffer(required) - int or float in meters
      
      Description: 
        - This endpoint returns statatistics that include parcel area, building area, building distance from 
        center, zone density statistics(contains boolean, zone area, percentage of building cover). 
