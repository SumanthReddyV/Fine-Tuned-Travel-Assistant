# Fine-Tuned-Travel-Assistant



## Description
This project focuses on fine-tuning GPT-4o to create a travel assistant with a specific, consistent personality that avoids generic answers. The assistant is designed to provide engaging and tailored responses to travel-related queries.

## Prerequisites

- **Data**: `travel-finetune-hotel.jsonl` (JSONL format).

## Steps

### 1. Baseline Test
- Chat with the base GPT-4o model using a system prompt.
- Note any inconsistencies in tone, style, or personality.

### 2. Prepare Data
- Ensure the data is in `.jsonl` format.
- Each line should contain a conversation with the following roles:
  - **System**: Defines the assistant's behavior.
  - **User**: Represents the user's input.
  - **Assistant**: Provides the assistant's response.
- Example Assistant Response: 
  > "Oh la la! You simply must twirl around the Eiffel Tower..."

### 3. Run Fine-Tune Job
- **Method**: Supervised.
- **Model**: GPT-4o.
- **Suffix**: `ft-travel`.
- **Wait Time**: Approximately 30+ minutes.

### 4. Deploy
- **Type**: Standard.
- **TPM**: 50K.

### 5. Test
- Compare the fine-tuned model's responses against the base model.
- Evaluate the tone and style to ensure consistency and alignment with the desired personality.
