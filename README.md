version: "3.1"

intents:
  - greet
  - goodbye
  - affirm
  - deny
  - mood_great
  - mood_unhappy
  - bot_challenge
  - recommend_movie
  - get_movie_by_imdb_rating
  - get_movie_by_title
  - get_movie_by_genre
  - get_movie_by_Runtime
  - get_movie_description

responses:
  utter_greet:
  - text: "Hey! How are you?"

  utter_cheer_up:
  - text: "Here is something to cheer you up:"
    image: "https://i.imgur.com/nGF1K8f.jpg"

  utter_did_that_help:
  - text: "Did that help you?"

  utter_happy:
  - text: "Great, carry on!"

  utter_goodbye:
  - text: "Bye"

  utter_iamabot:
  - text: "I am a bot, powered by Rasa."
   
  utter_recommend_movie:
  - text: "Sure! I recommend the movie '{title}'."

  utter_get_movie_by_imdb_rating:
  - text: "I will show you the imdb rating of that movie'{title}."
  
  utter_get_movie_by_title:
  - text: "Sure! I recommend the movie '{title}'."

  utter_get_movie_by_genre:
  - text: "Sure! I will recommend some movies by gender {genre}."

  utter_get_movie_by_Runtime:
  - text: "Sure! I'm gonna show you the runtime for that movie {runtime}."

  utter_get_movie_description:
  - text: "Of course. I will show you the description of the movie based on his name (title)."


session_config:
  session_expiration_time: 60
  carry_over_slots_to_new_session: true
