# Data set link
[Traffic Classification Dataset](https://drive.google.com/drive/folders/1qybhWvHUMh9ar4MZCaSCh65jn4U3Kg3q?usp=sharing)


# About

Traffic sign classification is an important task for self driving cars.
The dataset contains 43 different classes of images.  Images are 32 x 32 pixels

Classes are as listed below: 

1. 0 = Speed limit 20km/h
2. 1 = Speed limit 30km/h
3. 2 = Speed limit 50km/h
4. 3 = Speed limit 60km/h
5. 4 = Speed limit 70km/h
6. 5 = Speed limit 80km/h
7. 6 =End of Speed limit 80km/h
8. 7 = Speed limit 100km/h
9. 8 = Speed limit 120km/h 
10. 9 = No passing 
11. 10 = No passing for vehicles over 3.5 metric tons 
12. 11 = Right-of-way at the next intersection
13. 12 = Priority road
14. 13 = Yield
15. 14 = Stop
16. 15 = No vehicles
17. 16 = Vehicles over 3.5 metric tons prohibited
18. 17 = No entry
19. 18 = General caution 
20. 19 = Dangerous curve to the left
21. 20 = Dangerous curve to the right
22. 21 = Double curve
23. 22 = Bumpy road 
24. 23 = Slippery road
25. 24 = Road narrows on the right 
26. 25 = Road work
27. 26 = Traffic signals 
28. 27 = Pedestrians 
29. 28 = Children crossing
30. 29 = Bicycles crossing
31. 30 = Beware of ice/snow
32. 31 = Wild animals crossing
33. 32 = End of all speed and passing limits 
34. 33 = Turn right ahead
35. 34 = Turn left ahead 
36. 35 = Ahead only 
37. 36 = Go straight or right
38. 37 = Go straight or left 
39. 38 = Keep right 
40. 39 = Keep left
41. 40 = Roundabout mandatory 
42. 41 = End of no passing
43. 42 = End of no passing by vehicles over 3.5 metric tons

## LeNet architecture

LeNet was presented by Yann LeCun

### LeNet Layers
1. THE FIRST CONVOLUTIONAL LAYER #1
	
	Input = 32x32x1 
	
	Output = 28x28x6 
	
	Output = (Input-filter+1)/Stride* => (32-5+1)/1=28 
	
	Used a 5x5 Filter with input depth of 3 and output depth of 6 
	
	Apply a RELU Activation function to the output 
	
	pooling for input
	Input = 28x28x6 and Output = 14x14x6 

2.  THE SECOND CONVOLUTIONAL LAYER #2
	
	Input = 14x14x6 
	
	Output = 10x10x16 
	
	Layer 2: Convolutional layer with Output = 10x10x16 
	
	Output = (Input-filter+1)/strides => 10 = 14-5+1/1 
	
	Apply a RELU Activation function to the output 
	
	Pooling with Input = 10x10x16 and Output = 5x5x16 

3. STEP 3: FLATTENING THE NETWORK

	Flatten the network with Input = 5x5x16 and 
	Output = 400 

4. STEP 4: FULLY CONNECTED LAYER

	Layer 3: Fully Connected layer with Input = 400 and Output = 120 

	Apply a RELU Activation function to the output 

5. STEP 5: ANOTHER FULLY CONNECTED LAYER
	
	Layer 4: Fully Connected Layer with Input = 120 and Output = 84 
	
	Apply a RELU Activation function to the output 

6. STEP 6: FULLY CONNECTED LAYER
	
	Layer 5: Fully Connected layer with Input = 84 and Output = 43




