# langchain-output-parsers-demo
A hands-on project demonstrating the usage of different output parsers in LangChain — including StrOutputParser, JsonOutputParser, PydanticOutputParser, StructuredOutputParser, and CommaSeparatedListOutputParser — using OpenAI models in Python. Perfect for learning how to structure and validate LLM outputs in real-world applications.

````markdown
# 🧠 LangChain Output Parsers Demo

This project is a hands-on exploration of **LangChain's output parsers**, designed to convert raw, unstructured LLM outputs into structured formats like strings, lists, dictionaries, and Pydantic models. It's perfect for understanding how to work with **LLMs in production-grade applications**.

---

## 📌 What This Project Covers

In this notebook-based demo (Colab), you’ll learn how to:

✅ Use various types of output parsers in LangChain  
✅ Convert raw LLM output into clean Python objects  
✅ Design prompts that align with parser instructions  
✅ Validate and parse structured responses using Pydantic  
✅ Build modular LLM chains using `PromptTemplate`, `LLM`, and `OutputParser`

---

## 🧠 Skills I Learned

- 🧱 **Prompt Engineering**: Creating prompts compatible with parser instructions  
- 🧪 **Data Parsing**: Extracting and validating structured output from LLMs  
- 📦 **LangChain Core Usage**: Using LCEL (`|` composition), `PromptTemplate`, and `invoke()`  
- 🛠 **Pydantic Validation**: Creating typed models and validating data  
- 🔄 **Partial Prompt Filling**: Using `.partial()` to pre-fill prompt variables  
- 📊 **Hands-on Practice with OpenAI Models** (like `gpt-3.5-turbo`, `gpt-4o`)  

---

## 📦 Output Parsers Covered

| Parser Type                  | Description                                                                 |
|-----------------------------|-----------------------------------------------------------------------------|
| `StrOutputParser`           | Returns the raw string output as-is                                         |
| `CommaSeparatedListOutputParser` | Converts text to a Python list split by commas                        |
| `JsonOutputParser`          | Parses the output into a valid JSON object                                  |
| `PydanticOutputParser`      | Parses and validates output against a custom Pydantic model                 |
| `StructuredOutputParser`    | Similar to Pydantic parser, but generates `format_instructions` from schema |

---

## 🚀 How to Run the Project

1. Open the notebook in [Google Colab](https://colab.research.google.com/) or locally.
2. Install dependencies:
   ```bash
   pip install langchain langchain_openai langchain_core pydantic
````

3. Add your OpenAI key using:

   ```python
   import os
   os.environ["OPENAI_API_KEY"] = "your-key-here"
   ```

## 📁 File Structure

```
📁 langchain-output-parsers-demo/
│
├── OutputParsersDemo.ipynb          # Your Colab notebook with working examples
├── README.md                        # You're reading it 🙂
└── requirements.txt                 # (Optional) dependencies list
```

---

## 🏁 Conclusion

This project helped reinforce key LangChain concepts like output parsing, prompt structuring, and working with LLM pipelines. You can now confidently parse model responses and apply them to structured use cases like:

* Resume parsing
* AI form filling
* JSON API generation
* Knowledge base lookups
* and more!

---

## 🪪 License

MIT License. Feel free to fork, use, and build upon this demo.

---

## 🙌 Acknowledgements

Built as part of my self-learning journey into LangChain and LLM engineering. Special thanks to the LangChain docs and open-source community!

```
