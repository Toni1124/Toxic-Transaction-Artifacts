# Prompts Template
Prompt templates for semantically meaningful content extraction.

```
System: You are a helpful assistant.

User: Please help me determine whether the input text is meaningful. No explanation is needed, just return "yes" or "no". When making the judgment, please pay attention to the following points:
1. Code is meaningful.
2. Any human-readable content in any language is meaningful. Example: Й BcÃě Жe, Я ДaЖe He бyДy HиЧeГОnиcaть ИeЛый ToД.
3.Records without explanation or contain too little information are not meaningful. Meaningless example:=:BNB.BNB:bnb13vzla9uv4myxs0xrgtd4kheszz25i855ricmm2:3311061:te:0

Input text: {A text segment obtained from the first-phase filtering}

```