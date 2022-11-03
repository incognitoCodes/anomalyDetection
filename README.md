# Anomaly Detection
Anomaly detection using SageMaker built-in algorithm - Random Cut Forest

Amazon SageMaker Random Cut Forest (RCF) is an algorithm designed to detect anomalous data points within a dataset. Examples of when anomalies are important to detect include when website activity uncharactersitically spikes, when temperature data diverges from a periodic behavior, or when changes to public transit ridership reflect the occurrence of a special event.

In this notebook, we will use the SageMaker RCF algorithm to train an RCF model on the Numenta Anomaly Benchmark (NAB) NYC Taxi dataset which records the amount New York City taxi ridership over the course of six months. We will then use this model to predict anomalous events by emitting an "anomaly score" for each data point. The main goals of this notebook are,

to learn how to obtain, transform, and store data for use in Amazon SageMaker;
to create an AWS SageMaker training job on a data set to produce an RCF model,
use the RCF model to perform inference with an Amazon SageMaker endpoint.