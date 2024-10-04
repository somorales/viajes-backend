

# TravelStories

This repository is a [json-server](https://github.com/somorales/viajes-backend) created to feed data into the React Application below.

#### [Client Repo here](https://github.com/somorales/Viajes)

# Server Structure

## Collections

### cities

```javascript
{
  city,
  country,
  tip,
  fact,
  image,
  stamps,

}
```

### recommendations

```javascript
 {
   title,
   description,
   date,
   companion,
   usuario,
   category,
   image,
   stamp,
 }
```

## Used API Endpoints in the App

| HTTP Method | URL                                              | Component                                | Description                                                    |
| ----------- | ------------------------------------------------ | ---------------------------------------- | -------------------------------------------------------------- |
| GET         | `/`                                              | `<HomePage cities={cities} />`           | Displays the home page with a list of all cities                |
| GET         | `/:city`                                         | `<CityRecommendations cities={cities} favs={favs} setFavs={setFavs}/>` | Displays recommendations for a specific city                   |
| GET         | `/:city/:cityId/recommendations/:recommendationId` | `<RecommendationDetails />`              | Displays details for a specific recommendation                  |
| PUT         | `/:city/:cityId/recommendations/:recommendationId` | `<EditRecommendation />`                 | Edit a specific recommendation from the details page            |
| POST        | `/create`                                        | `<CreateRecommendation cities={cities} />` | Form to create a new recommendation for a city                  |
| GET         | `/about`                                         | `<About />`                              | Displays the "About" page with info on the app                  |
| DELETE      | `/:city/:cityId/recommendations/:recommendationId` | `<RecommendationDetails />`              | Delete a specific recommendation                               |
| GET         | `/preview`                                       | `<CardPreview />`                        | Preview a recommendation card                                  |
| GET         | `*`                                              | `<Error />`                              | Displays an error page for unmatched routes                    |
| GET         | `/favs`                                          | `<Favs favs={favs} setFavs={setFavs} />` | Displays a list of favorite recommendations                    |



## Links

### Collaborators

[Angela Ruiz](https://github.com/anruiz-r)

[Sofia Morales](https://github.com/somorales)

### Project

[Repository Link Client](https://github.com/somorales/Viajes)

[Repository Link Server](https://github.com/somorales/viajes-backend)

[Deploy Link](https://travelstories-as.netlify.app/)

### Trello

[We use trelo to plan the project.](https://trello.com/b/H3SqggjI)

### Slides

[Demo](https://www.figma.com/board/4sVdUtalSetB9V07HbKqwa/TravelStories?node-id=0-1&node-type=canvas&t=LUjbhfQEYBU4J3mw-0)