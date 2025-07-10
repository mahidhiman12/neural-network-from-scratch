# neural-network-from-scratch
Neural network built completely from scratch using NumPy - includes dropout, L2 regularization, and Adam optimizer

# Neural Network from Scratch (NumPy Only)

Built a full neural network **from scratch** using only NumPy — no TensorFlow, no PyTorch, no frameworks. Just raw Python, and maths.  
Includes:
- Dropout regularization
- L2 weight regularization
- Adam optimizer
- Forward + backward pass
- Decision boundary visualization

 Built this to truly understand *how neural nets learn*.


##  Problem Statement is:

This project tackles a **multiclass classification** problem using a synthetic spiral dataset.

Each data point:
- Has two input features: `x1`, `x2`
- Belongs to one of **three classes**:  
  🔴 Red, 🟢 Green, 🔵 Blue

###  Goal:  
Design a neural network that can take any new input point (x1, x2) and **accurately classify** it into the correct class (red/green/blue).

Sounds simple? The data is **non-linearly separable**, so linear models won’t cut it — this is where neural nets shine.

---

##  Model Architecture

```text
Input (x1, x2)
   ↓
Dense Layer (64 units)
   ↓
ReLU Activation
   ↓
Dropout (rate=0.05)
   ↓
Dense Layer (3 units)
   ↓
Softmax + Categorical Crossentropy Loss
