* Task 2: Explore Min, Max, and Median filters and apply those filters on noisy images and
write
* 
1. Purpose of each filter 
2. Your experimental results 
3. Observations 4. Change
kernel sizes and observe differences.

* OUTPUT:
* 
On nomal image:
Here I am adding noise in the image manually
<img width="624" height="225" alt="image" src="https://github.com/user-attachments/assets/8986a600-f8fd-4a1d-a370-cb88af8682e5" />
<img width="624" height="223" alt="image" src="https://github.com/user-attachments/assets/eff0dbfc-484c-4f26-a5f2-64d6140aa30c" />
On salt&Peper noise:  (the original = Noisy imges )
<img width="624" height="225" alt="image" src="https://github.com/user-attachments/assets/ce2715cc-5592-4d42-954b-d61c38e4347b" />
<img width="624" height="218" alt="image" src="https://github.com/user-attachments/assets/e25ad170-943a-4d26-a968-457f545a208a" />
* Q&A: 
*
 1. Purpose of Each Filter
# Median Filter
•	Removes salt-and-pepper noise 
•	Replaces pixel with median value 
•	Preserves edges 
________________________________________
# Min Filter (Erosion)
•	Replaces pixel with minimum value in neighborhood 
•	Removes bright noise (salt noise) 
•	Darkens the image 
________________________________________
# Max Filter (Dilation)
•	Replaces pixel with maximum value 
•	Removes dark noise (pepper noise) 
•	Brightens the image 
________________________________________
 # 2. Experimental Results
•	Median filter successfully removed most noise. 
•	Min filter removed bright pixels but made image darker. 
•	Max filter removed dark pixels but made image brighter. 
•	Increasing kernel size increased smoothing effect. 
________________________________________
# 3. Observations
•	Median filter gives best visual quality. 
•	Min filter shrinks bright regions. 
•	Max filter expands bright regions. 
•	Larger kernels: 
o	Remove more noise 
o	But reduce image details
________________________________________
 # Which filter blurs the image the most?
Median filter with large kernel (e.g., 7×7)
Because it replaces values using neighborhood sorting → strong smoothing.
________________________________________
 # Which filter preserves edges better?
Median filter
Because it does not average values — it selects actual pixel values.
-------------------------------------------
# Final Conclusion 

The median filter proved to be the most effective for removing salt-and-pepper noise while preserving image details. Increasing kernel size improves noise removal but reduces sharpness.
Min and max filters are limited to specific noise types and degrade overall image quality.