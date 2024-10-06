# Seismic Detection
We developed algorithmic and machine learning models to identify seismic events in real data from the Apollo missions and the Mars InSight mission, minimizing the transmission of unnecessary information. For the Moon, we applied traditional signal processing techniques like Fast Fourier Transform and spectrogram analysis to detect seismic events, achieving reasonable accuracy. For Mars, where the signal-to-noise ratio is lower, we used advanced machine learning, specifically a long short term memory model, to handle the time-series nature of seismic data. This model captures subtle temporal patterns and dependencies, helping to predict the timing of seismic events. Though the accuracy of the machine learning model was lower due to potential noise sensitivity, it offers a scalable solution that can be improved with further refinement. Our models help improve seismic event detection and enhance data efficiency and advance our understanding of planetary activity. 

## Additional data
This Google Drive contains data that we used for our project. 
https://docs.google.com/document/d/11yPrLIqcA9FDIywRGnuaOL1iYACTb3Usb5KmRUoA8ms/edit?usp=sharing

## Project Details
Planetary seismology missions face significant challenges with power limitations, particularly when transmitting continuous seismic data from distant planets back to Earth. Given that only a fraction of the data is scientifically useful, optimizing data transmission is critical. This project aims to address this issue by developing a computer program capable of distinguishing between noise and scientifically valuable seismic signals. By analyzing real data from the Apollo missions and the Mars Interior Exploration using Seismic Investigations, the goal is to identify and extract seismic events, minimizing the need to send back unnecessary information. 

In developing our project, we used Google Colab as the primary development environment and Python as the primary programming language. We decided to use different algorithms for Moon and Mars predictions, because of the differences in signal-to-noise ratio and the amount of data that was available for training. 
We created a webpage to present our results, and to display our results more efficiently, we created interactive plots for visualization. For creating interactive plots, we used Holoviews, a high-level data visualization library that simplifies the creation of interactive plots, and Panel, a powerful tool for building interactive web applications and dashboards in Python. The interactive plot displays continuous seismic records as curves over time with event markers. By hovering on the curve, users can retrieve information about the relative time and amplitude at that point. The user can also zoom in and out on specific sections of the data using the zoom box, time sliders and amplitude sliders. After doing some visual manipulations, the user can also save the plot as an image.

We approached this challenge by the following methods:
<ol>
  <li>Algorithmic Predictive Models</li>
  <li>Machine Learning Model</li>
</ol>
