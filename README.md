# NILM ML project

Non-intrusive load monitoring(NILM) is the task of separating the total household energy measured into its constituent appliances. An open-source NILM toolkit called NILMTK was developed in 2014 to make NILM research reproducible and to ensure easy comparison of benchmark NILM algorithms. With the addition of more algorithms like Seq2Seq, Seq2Point models and improvements in both the experiment and model interface, an improved version of the toolkit NILM-contrib was released in 2019. However, the existing neural network models in the toolkit do not capture the model uncertainty. This project aims to add the uncertainty prediction component using MC dropout method to the existing state-of-the-art Seq2Point
model and then to the Seq2Seq model.

In this project, we implemented MC Dropout method on the top
of Seq2Seq and Seq2Point algorithm. We tuned the hyper param-
eters dropout rate and the number of iterations used during the
prediction phase. We observed a drop out rate of 0.2 and number
of iteration of 100 is optimum for the models. Then we quantified the uncertainties of Seq2Seq and Seq2Point models (our implementation) using calibration plots. Seq2Point model performed better than Seq2Seq model in uncertainty predictions since miscalibrated area in calibration plot is less for all appliances for Seq2Point in comparison to Seq2Seq.


Team Members:

1. Akshat Mangal
2. Gaurav Sonkusle
3. Mohamed Shamir
4. Mohmmad Aslam
5. Keyur Unadkat
