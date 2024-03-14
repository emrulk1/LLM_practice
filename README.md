# OpenOrca Dataset

## Dataset Summary

The OpenOrca dataset comprises augmented data from the FLAN Collection, including approximately 1 million GPT-4 completions and 3.2 million GPT-3.5 completions. It is structured in alignment with the distributions outlined in the ORCA paper and represents a partial fulfillment of the complete dataset envisioned, with ongoing efforts to expand its scope. This dataset is primarily employed for training and evaluation purposes within the field of natural language processing (NLP).

## Dataset Attribution

Special recognition is extended to the following contributors for their considerable efforts and dedication:

- Teknium
- WingLian/Caseus
- Eric Hartford
- NanoBit
- Pankaj
- Winddude
- Rohan

Additional thanks to http://AlignmentLab.ai for contributions from:

- Autometa
- Entropi
- AtlasUnified
- NeverendingToast
- NanoBit
- WingLian/Caseus

## Supported Tasks and Leaderboards

OpenOrca supports various tasks, including language modeling, text generation, and text augmentation. It has played a crucial role in generating multiple high-performing model checkpoints, demonstrating exceptional performance in unit testing. Updates on leaderboards and further information will be provided as available.

## Languages

The dataset is primarily in English.

## Dataset Structure

### Data Instances

Each instance in the dataset is an entry from the FLAN collection, augmented by submitting the listed question to either GPT-4 or GPT-3.5, with the response recorded in the response field.

### Data Fields

- `id`: A unique numbered identifier, including tags like 'niv', 't0', 'cot', or 'flan' to denote the source FLAN Collection submix.
- `system_prompt`: The System Prompt presented to the GPT-3.5 or GPT-4 API.
- `question`: A question entry from the FLAN Collection.
- `response`: The response to the question received from a query to either GPT-3.5 or GPT-4.

### Data Splits

The dataset is currently unsplit.

## Dataset Creation

### Curation Rationale

OpenOrca was curated to serve as an augmented text data source for researchers and developers, enhancing the core FLAN Collection data with detailed reasoning traces from GPT-3.5 and GPT-4. This augmentation has yielded exceptional results, particularly in hard reasoning tasks.

### Source Data

The data generation adheres to the distributions specified in the Orca paper, with notable exceptions regarding the CoT data. The dataset uses pre-generated FLAN Collection datasets hosted on HuggingFace as its primary data source.

## Dataset Use

### Use Cases

OpenOrca is suitable for tasks related to language understanding, natural language processing, machine learning model training, and evaluation.

### Usage Caveats

As a work-in-progress, users are advised to check for dataset updates and improvements. The dataset should be utilized following the Orca paper's guidelines and recommendations.

### Getting Started

The dataset is designed for easy loading via the Hugging Face datasets library, with streaming recommended due to file sizes. For updates and progress, monitor the OpenOrca repository on Hugging Face.

