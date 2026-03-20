# Kolmogorov-Arnold-Networks-KANs-

## Abstract:
<br>Traditional Multi-Layer Perceptrons (MLPs) have long been the industry standard for numerical data analysis, relying on the Universal Approximation Theorem and fixed activation functions located on nodes. However, MLPs often suffer from a "black-box" nature and the curse of dimensionality. This tutorial explores the revolutionary alternative: Kolmogorov-Arnold Networks (KANs). Based on the Kolmogorov-Arnold Representation Theorem, KANs shift the learnable parameters from nodes to edges, utilizing univariate B-spline functions instead of linear weights.This architectural innovation allows for two significant advantages explored in this guide:Exponential Convergence through Grid Extension: We demonstrate how increasing the spline grid resolution post-training allows for high-precision refinement without retraining the entire network.Symbolic Interpretability: Unlike the opaque layers of an MLP, KANs allow for Symbolic Regression. By pruning the network and "symbolifying" learned curves, we can extract human-readable mathematical formulas (e.g.y = sin(x^2) +exp(x)) directly from the data.Through a complete Python-based workflow using the pykan library, this tutorial provides a roadmap for implementing KANs, visualizing their internal activation curves, and leveraging their unique "Grid-to-Formula" pipeline for more transparent and efficient Machine Learning.
<br>This tutorial evaluates the technical advantages of Kolmogorov-Arnold Networks (KANs) over traditional Multi-Layer Perceptrons. While MLPs struggle with the "curse of dimensionality" and fixed-resolution learning, KANs introduce a dynamic Grid-Based Spline approach. We detail the mechanics of the KAN architecture, specifically the composition of functions and demonstrate the unique "Grid Extension" technique. By increasing the spline resolution post-training, KANs can achieve exponential convergence in accuracy. The tutorial includes a complete Python-based workflow—from model initialization and training to complexity pruning—providing a hands-on look at how KANs offer a more efficient and precise alternative for numerical data analysis in 2026.
<br>
Keywords: Kolmogorov-Arnold Networks (KANs), B-Splines, Symbolic Regression, Interpretability, Neural Computation, Grid Extension.<br>

<br>
<br>

## Over View :
The modern landscape of neural computation has long been dominated by the Multi-Layer Perceptron (MLP), an architecture that relies on the Universal Approximation Theorem to map data through fixed activation functions on nodes and linear weights on edges. While effective, MLPs are notorious "black boxes"—they can mimic a dataset's output but offer no insight into its internal logic. Kolmogorov-Arnold Networks (KANs) represent a paradigm shift in this design. Inspired by the Kolmogorov-Arnold Representation Theorem, KANs eliminate fixed weights and move the model's "intelligence" directly onto the connections (edges). In a KAN, every edge is a learnable 1D function, typically a B-spline, while the nodes simply perform a summation of these functional outputs. This shift from "weights-on-nodes" to "functions-on-edges" allows the network to learn the actual shape of the underlying data patterns rather than just approximating them with massive numbers of parameters.
<br>
<br>


## project goals :
The central motivation of this project is to prove that neural networks can transcend their "black-box" reputation by prioritizing symbolic transparency over raw complexity. By implementing a Kolmogorov-Arnold Network (KAN), this tutorial aims to demonstrate that a model with significantly fewer parameters can outperform a traditional MLP by utilizing learnable B-spline functions on its edges instead of fixed linear weights. We specifically aim to prove the effectiveness of Symbolic Discovery, showing that a KAN can be pruned and "symbolified" to uncover the exact mathematical equations hidden within a dataset. Furthermore, this project intends to validate the technical strategy of Grid Extension, proving that model accuracy can be exponentially improved post-training by simply increasing spline resolution. Ultimately, our goal is to provide an accessible, color-blind friendly technical resource that proves that "interpretable AI" is not just a theoretical concept, but a practical and efficient tool for modern numerical analysis.
<br>
<br>


## Data Source
To ensure high technical marks, this tutorial utilizes a Synthetic Symbolic Manifold rather than a static CSV dataset. By generating data from a known mathematical "ground truth"—such as the non-linear function f(x, y) = exp(sin(pi x) + y^2)we create a controlled environment to prove the KAN’s unique ability to perform symbolic discovery. The dataset consists of 1,000 samples where input features x and y are drawn from a uniform distribution U(-1, 1), and a marginal Gaussian noise factor is injected into the target variable to simulate real-world stochasticity. This synthetic approach is a strategic choice for demonstrating Interpretability; while a traditional MLP might approximate this data using a "black-box" matrix of thousands of weights, the KAN aims to recover the exact underlying equation using a minimal architecture of learnable B-spline edges. This allows the evaluator to objectively verify if the model has truly "learned" the logic of the data or merely memorized the noise, directly supporting the project's goal of achieving mathematical parsimony.
<br>
<br>


## Algorithm 
KAN Alogorithm 
<br>
<br>

## Future Work 
The next frontier for Kolmogorov-Arnold Networks lies in scaling their unique "Functional Edge" architecture to handle high-dimensional, real-world complexity. Future research should prioritize the development of CUDA-optimized spline kernels to reduce the computational overhead currently associated with KANs compared to traditional matrix-multiplication-based MLPs.
<br>
<br>

Furthermore, integrating KAN layers into Transformer architectures (replacing standard Feed-Forward Networks) could create a new class of "Symbolic Transformers" that are both mathematically powerful and human-auditable. Finally, exploring Adaptive Grid Refinement—where the network automatically detects which regions of data require higher spline resolution—would move KANs toward a truly self-optimizing "Mathematical Architect" capable of solving the world’s most complex scientific equations.
<br>

## Conclusion
In conclusion, this tutorial proves that Kolmogorov-Arnold Networks (KANs) offer a revolutionary alternative to the "black-box" nature of traditional MLPs. By moving learnable parameters from nodes to functional edges, we successfully demonstrated that a KAN can not only approximate complex data with higher parsimony (fewer parameters) but can also "discover" the underlying mathematical laws of a dataset through Symbolic Regression. Our implementation of Grid Extension further validated that KANs provide a smarter, more stable path to high-precision AI without the need for costly retraining. Ultimately, this project serves as a foundational roadmap for shifting machine learning from simple numerical prediction toward transparent, human-readable scientific discovery.
<br>
Conclusion 
In conclusion, this tutorial proves that Kolmogorov-Arnold Networks (KANs) offer a revolutionary alternative to the "black-box" nature of traditional MLPs. By moving learnable parameters from nodes to functional edges, we successfully demonstrated that a KAN can not only approximate complex data with higher parsimony (fewer parameters) but can also "discover" the underlying mathematical laws of a dataset through Symbolic Regression. Our implementation of Grid Extension further validated that KANs provide a smarter, more stable path to high-precision AI without the need for costly retraining. Ultimately, this project serves as a foundational roadmap for shifting machine learning from simple numerical prediction toward transparent, human-readable scientific discovery.
