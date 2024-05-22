## Vision Language Models and the future of the self driving car

Self driving cars have been a Silicon Valley darling for many years. Over $100 billion have been invested in this technology with very limited results. There is a whole load of examples of failures. 

# Where does the self driving car fail us?

So many examples! 

Take for example this classic example of a bus with an ad for a politician.  (I use this in my lectures). The self driving car - a tesla - sees the bus and thinks a man is walking behind it:


# What is wrong with the technology>

The last generation of models was based on supervised learning, but this might be a wrong approach. It takes tens of thousands of examples to train a specific model. That seems a lot, but might still not be enough. 

So for example to learn a car to detect the STOP sign, you collect many images, label the images, train a model and the car will detect the STOP sign. Works very nice, in the lab that is.  

# Where the stop sign goes wrong

Take for example this guy on instagram. He wears a t-shirt with a stop sign. Guess what the self-driving taxi does? It recognises the stop sign and stops. WRONG! It couldn't make a distinction between a t-shirt and a real traffic sign. 


![Insta post by jasonbcarr](https://www.instagram.com/reel/C5O_hV8v9bi/?utm_source=ig_embed?raw=true)



# Vision Language Models to the rescue! 
Recently a new class of models have become very popular: Vision Language Models. These models are a combination, as the name suggests, of vision and language. 

It takes an image as input and it describes the image for you. So, in our example of a guy wearing a t-shirt with a stop sign on it it gives the following result:

"The man in the image is standing on the sidewalk, wearing a hat and a stop sign shirt." (Model = Kosmos-2) This  model can make the distinction between a real traffic sign and a man wearing at funny t-shirt! 

Try this yourself at https://huggingface.co/spaces/merve/compare_VLMs 

Try my notebook on the subject so you can see for yourself:

https://github.com/MichielBbal/ollama/blob/main/ollama_llava_self_driving_car.ipynb 