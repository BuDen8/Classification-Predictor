# Classification-Predictor
Trained a Random Forest algorythm to predict when the outcome of an event will be 1 or 0 based on given features.

This is still a WIP!

While working in Wayfair I had the opportunity to develop a Random Forest algorythm that would predict whether an order that is coming to one of our warehouses will be delivered late to our customers based on readily available features such as: the volume of that warehouse in the last 48h, the warehouse within our network processing the order, the number of people required to process the order based on size.


The current model is able to predict with 76% accuracy (0.8 AUC) whether an order will be delivered late or not. The next steps are:
  1.Build a data pipeline to provide real-time live order data to the model in order to make real time predictions
  2.Create a pickle file where the model can be stored and used for new predictions.
  3.Create a performance tracking dashboard that would allow users to better understand and what point in the order cycle does the model predict best.
  4.Surface predictions in Data Studio dashboard for warehouses to use on a daily basis in order to make prioritization of orders.
