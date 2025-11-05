# Polimi Master Thesis

## Title: Concept-Based Explanations for Image Classifiers using Textual Prompts

This thesis proposes a scalable approach to enhance the transparency of Convolutional Neural Networks (CNNs) in the field of Explainable Artificial Intelligence (XAI).

Leveraging the multimodal model CLIP, we compute latent representations of arbitrary Concepts from textual inputs. These concept embeddings are then used to inspect and interpret the internal mechanisms of any CNN model.

This approach provides greater control over the knowledge learned by CNNs, offering applications that go beyond explainability.

Moreover, concepts can also be employed for localization tasks: by filtering CNN features to retain only those relevant to a given concept, we can generate heatmaps or bounding boxes highlighting the regions of the image that express that concept.

## Abstract

TCAV and its extension Visual-TCAV represent the current state of the art among Concept-based Explainable AI (XAI) methods for Image Classifiers. However, these methods suffer from a limitation: they are not easily scalable. In fact, the extraction of a CAV requires a large number of images illustrating the concept, making the process labor-intensive and time-consuming. We propose a novel solution to extract CAVs directly from textual inputs. Our approach leverages the multimodal capabilities of CLIP to generate embeddings from text, which we then align to the latent space of a CNN via a simple linear model. This produces a concept embedding compatible with Visual-TCAV, enabling textual concept- based explanations. Furthermore, we extend the use of CAVs beyond the field of XAI into the domain of visual localization. We demonstrate that it is possible to perform zero-shot localization tasks by using only the object’s CAV obtained via text, along with the feature maps extracted from the CNN. Specifically, we can generate bounding boxes for generic objects, without the need for a specific training.
