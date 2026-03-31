# 🧪 Task 2: Image De-Noising using Min, Max & Median Filters

This experiment explores the effect of **Min, Max, and Median filters** on noisy images, along with analysis of their behavior, performance, and impact on image quality.

---

## 🎯 Objectives

* Apply different filters on noisy images
* Analyze their performance
* Study the effect of **kernel size**
* Compare results visually and conceptually

---

## 🖼️ OUTPUT

### 🔹 On Normal Image (Noise Added Manually)

Here, artificial noise is added to a clean image to observe filter performance.

<img width="624" height="225" alt="image" src="https://github.com/user-attachments/assets/8986a600-f8fd-4a1d-a370-cb88af8682e5" />
<img width="624" height="223" alt="image" src="https://github.com/user-attachments/assets/eff0dbfc-484c-4f26-a5f2-64d6140aa30c" />

---

### 🔹 On Salt & Pepper Noise

*(Here, the original image is treated as noisy input)*

<img width="624" height="225" alt="image" src="https://github.com/user-attachments/assets/ce2715cc-5592-4d42-954b-d61c38e4347b" />
<img width="624" height="218" alt="image" src="https://github.com/user-attachments/assets/e25ad170-943a-4d26-a968-457f545a208a" />

---

## 📌 1. Purpose of Each Filter

### 🔸 Median Filter

* Removes **salt-and-pepper noise**
* Replaces pixel with **median value**
* Preserves edges effectively

---

### 🔸 Min Filter (Erosion)

* Replaces pixel with **minimum value in neighborhood**
* Removes **bright (salt) noise**
* Makes image **darker**

---

### 🔸 Max Filter (Dilation)

* Replaces pixel with **maximum value**
* Removes **dark (pepper) noise**
* Makes image **brighter**

---

## 📊 2. Experimental Results

* ✅ Median filter successfully removed most of the noise
* ⚠ Min filter removed bright pixels but made the image darker
* ⚠ Max filter removed dark pixels but made the image brighter
* 📈 Increasing kernel size increased smoothing effect

---

## 🔍 3. Observations

* ✔ Median filter provides the **best visual quality**
* ✔ Min filter **shrinks bright regions**
* ✔ Max filter **expands bright regions**

### 🔹 Effect of Kernel Size

* Small kernel (3×3):

  * Less smoothing
  * More details preserved

* Large kernel (7×7):

  * More noise removal
  * Loss of fine details (blurring)

---

## ❓ Key Questions & Answers

### 🔹 Which filter blurs the image the most?

👉 **Median filter with large kernel (e.g., 7×7)**
Because it performs strong smoothing using neighborhood values.

---

### 🔹 Which filter preserves edges better?

👉 **Median filter**
Because it selects actual pixel values instead of averaging.

---

## 🧾 Final Conclusion

The **Median filter** proved to be the most effective for removing **salt-and-pepper noise** while preserving important image details.

Although increasing the kernel size improves noise removal, it also introduces **blurring and loss of sharpness**.

Min and Max filters are limited in functionality:

* Min filter is useful for removing **bright noise**
* Max filter is useful for removing **dark noise**

However, both degrade overall image quality when used alone.

---

> 🚀 *This experiment highlights the importance of choosing the right filter based on noise type and application requirements.*
