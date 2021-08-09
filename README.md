# movie-rec-engine-backend

Here you can find the Movie Recommendation engine backend Flask API code. 

I created this project to leverage the open-source [MovieLens dataset](https://grouplens.org/datasets/movielens/) and hopefully help people figure out what to watch next. Below is an illustration of what the engine will recommend if you enter the movie "Heat (1995)". You can also try it out based on your favourite movie on: [mynextmovie.ca](https://mynextmovie.ca).  

![image](https://user-images.githubusercontent.com/26292532/128757396-9f10b632-dbbf-4b7e-a431-cd308cc08c54.png)


## Get started

To run the Flask API, you will first need to download the similarity matrix file from here

```
https://drive.google.com/drive/folders/1FH6bWCcw1OoRf4QJaFaf4gIegIGSEx9r
```

and place **movie_similarity.csv** file into the root directory. Your code structure should look as follows:

![image](https://user-images.githubusercontent.com/26292532/128761706-172d52a1-6dcf-41be-979d-c97753bced21.png)


Next make sure you have the necessary libraries installed. For example, if you are using conda, you can create a separate environment and install necessary libraries as follows:

```
conda env 
```

**To run the API:**

```
python application.py
```

To Test the API, in a  separate terminal run the following:

```
curl -X POST http://0.0.0.0:80/recms -H 'Content-Type: application/json' -d '{"movie_title":"Heat (1995)"}'
```

If everything is working properly, you should see the following output/recommendations:



