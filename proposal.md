# Anime IMDB

## A Anime app thats inpired by IMDB

An app that allows a user to log their daily meditation and gratude journals. The app allows them to view, edit, and delete post from previous dates.

## Wire Frames

![image](assets/wireframe.png)



## User Stories

#### MVP Goals

- AAU I would want to be able to sign in to the website
- AAU I would want to be able to scroll through the varieties of animes on the website 
- AAU I would want to be able to fav an anime
- AAU I would want a good description of the anime.

#### Stretch Goals

- a comment system to give my feedback on the anime
- to be able to scroll through categories
- to be able to rate the anime myself like a rating button from 1-5 stars
- a authentication system


| Method | Route                   | Description                           | Handler   | Auth Required | Example Response                        |
|--------|-------------------------|---------------------------------------|-----------|---------------|-----------------------------------------|
| POST   | /signin                 | User sign-in                          | signin    | No            | Redirect to user's dashboard            |
| GET    | /animes                 | Retrieve all anime varieties          | getAll    | No            | JSON array of anime varieties           |
| POST   | /animes/:animeId/fav    | Favorite an anime                     | addToFav  | Yes           | Success message or updated user profile |
| GET    | /animes/:animeId/desc   | Get anime description                 | getDesc   | No            | JSON object with anime details          |
