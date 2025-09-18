# AI/LLM Learning Glossary

## Bias
In neural networks, a single numerical value added to each neuron's calculation to shift its "threshold" or tendency to activate. Like setting a default starting point - analogous to having a coat-wearing threshold of 20°F instead of 0°F. Each neuron has exactly one bias value. This is different from social bias - it's purely mathematical.

## Layer
A processing stage in a neural network, like a step in an assembly line. Each layer performs a specific type of analysis before passing results to the next layer. For example: Layer 1 might recognize basic word patterns, Layer 2 might identify parts of speech, Layer 12 might predict the next word. GPT-2 has 12 layers, GPT-3 has 96 layers.

## Modalities
Different types of data or input/output formats that AI models can work with. Examples include text, images, audio, video, and code. Modern AI models can often work across multiple modalities (like processing both text and images together).

## Neuron
A basic processing unit in a neural network that receives inputs, performs calculations, and produces an output. Think of it like a decision-making component with multiple weighted inputs, one bias value, and one output. Large language models contain millions or billions of neurons organized across layers.

## NLP (Natural Language Processing)
The field of AI focused on helping computers understand, interpret, and generate human language. Includes tasks like translation, sentiment analysis, text summarization, question answering, and conversation.

## Parameters
The umbrella term for all the learned numerical values in a neural network, including both weights and biases. When someone says "GPT-3 has 175 billion parameters," they're counting all the weights (the vast majority) plus all the bias values. These are learned automatically during training, not set by humans.

## Pipeline
In Hugging Face, the `pipeline()` function is a high-level tool that simplifies using pre-trained AI models. It handles all the complex preprocessing and postprocessing automatically. There are different types of pipelines for different modalities and tasks:
- **Text pipelines**: text-generation, sentiment-analysis, translation, summarization, question-answering
- **Image pipelines**: image-classification, object-detection, image-to-text
- **Audio pipelines**: speech-recognition, audio-classification, text-to-speech
- **Multimodal pipelines**: visual-question-answering (combining text and images)

Each pipeline type is optimized for its specific task and data type, but all work with the same simple interface.

## Transformer
The neural network architecture that revolutionized AI, especially NLP. The "T" in GPT stands for Transformer. Originally designed for language translation, it turned out to be incredibly versatile and now powers most modern LLMs, image generators, and other AI applications. One architecture that can handle many different tasks.

## Weights
The numerical values that determine how much influence one neuron's output has on another neuron's input - like connection strengths between neurons. Each connection between neurons has its own weight value. These are learned during training through millions of corrections. In the coat analogy, if bias is your overall coat threshold, weights are how much you care about temperature vs. wind vs. humidity vs. other factors.

## Zero-shot
A model's ability to perform a task without being specifically trained or fine-tuned on examples of that task. For example, a zero-shot classification pipeline can categorize text into labels it has never seen before (like "happy", "sad", "angry") just based on its general language understanding. The model can return probability scores for any list of labels you provide, even though it wasn't explicitly trained on those specific categories.
