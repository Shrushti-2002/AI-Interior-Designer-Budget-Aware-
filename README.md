# AI-Interior-Designer-Budget-Aware-

- An end-to-end Machine Learning + Computer Vision application that analyzes a room image and recommends budget-aware furniture based on the predicted room type.
Built with FastAPI for speed and scalability using gradio web interface app.

🚀 Features

- 📷 Upload a room image

- 🧠 Extract visual features using a pretrained CNN

- 🏡 Predict room type (bedroom, living room, office, kitchen, etc.)

- 🪑 Recommend furniture using a real dataset

- 💰 Optimize selections to stay within user-defined budget

- ⚡ Fast, lightweight web app using FastAPI

🛠️ Tech Stack

- Backend - FastAPI

- Computer Vision - PyTorch, ResNet50

- Data Handling - Pandas, NumPy

- Image Processing - Pillow, OpenCV

🧩 How It Works (Step-by-Step)

1️⃣ Image Feature Extraction

- A pretrained ResNet50 model extracts a visual embedding from the uploaded image.

- Transfer learning avoids training from scratch.

2️⃣ Room Type Prediction

- The embedding is mapped to one of the predefined room types:

bedroom, living room, office, kitchen, dining room,
bathroom, kids room, studio apartment, home gym

- The current implementation uses an embedding-based heuristic
(can be upgraded to a trained classifier or object detection).

3️⃣ Budget-Aware Optimization

- Each room has required furniture categories.

- Furniture is selected from the dataset using a greedy strategy
while staying within the budget.

4️⃣ Response

The API returns:

- Predicted room type

- Recommended furniture items

- Remaining budget

Gradio UI - https://8001812b37a2ba97d1.gradio.live
