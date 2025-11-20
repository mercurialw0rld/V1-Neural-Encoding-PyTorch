# V1-Neural-Encoding-PyTorch
# 🧠 NeuroAI: Modelado de la Corteza Visual con PyTorch

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-red)

## 📖 Descripción
Este proyecto explora la intersección entre la **Neurociencia Computacional** y el **Deep Learning**. El objetivo es modelar matemáticamente cómo las neuronas de la corteza visual primaria (V1) codifican la información sensorial (contraste de luz).

Utilizando el dataset de *Steinmetz et al.* (neuropixels en ratones), entrené modelos para predecir la tasa de disparo neuronal (*spiking rate*) basándose en estímulos visuales.

## 📊 Resultados Clave

### 1. Descubrimiento de Curvas de Sintonización (Tuning Curves)
La red neuronal (MLP) descubrió exitosamente que las neuronas de V1 poseen **preferencias de estímulo**.

> **Hallazgo:** La neurona analizada mostró una respuesta excitatoria hasta un contraste total de ~0.5, seguida de una inhibición (control de ganancia) en contrastes altos.
* **Factor de Fano ($F$):** Se calculó un $F \approx 2.0$.
* **Interpretación:** La neurona exhibe un comportamiento "Super-Poisson", indicando una variabilidad superior al azar, consistente con mecanismos de disparo en ráfagas (*bursting*).

## 🛠️ Tecnologías Usadas
* **PyTorch:** Construcción y entrenamiento de modelos (autograd, nn.Module).
* **NumPy & Pandas:** Manipulación de matrices de spikes y contrastes.
* **Matplotlib:** Visualización de datos científicos.
* **Dataset:** Steinmetz.
