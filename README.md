Simplifying Financial Reports with Generative AI: An Intelligent Summarization
& Visualization Tool
Financial reports are critical for decision-making but are notoriously complex—filled with
technical jargon, intricate tables, and verbose disclosures. For non-experts, students, and
even junior analysts, extracting meaningful insights from these documents can be time-
consuming and overwhelming. To address this challenge, we developed an AI-driven tool that
simplifies financial analysis through summarization, visualization, and interaction—powered
entirely by open-source, lightweight components.
The solution allows users to upload PDF-based financial statements, which are then parsed
to extract text. Using transformer-based models such as DistilBART and FLAN-T5, the tool
generates context-aware summaries via multiple prompting strategies: Zero-shot, Few-shot,
Chain-of-Thought (CoT), and Tree-of-Thought (ToT). These summaries are evaluated using
BLEU, ROUGE-L, and BERTScore metrics. CoT prompting emerged as the most effective,
offering the highest ROUGE-L and a strong semantic alignment, making it ideal for
downstream tasks like data visualization.
Visualization suggestions—such as revenue trends or segment breakdowns—are derived
from the best-performing summary and rendered using real financial data. These include line
charts, bar comparisons, and pie charts, offering users an intuitive view of key financial
metrics. Additionally, a fine-tuned RoBERTa-powered chatbot allows users to ask natural
language questions and receive direct answers from the report, enhancing interactivity.
While the prototype operates within Google Colab’s free tier, it demonstrates the powerful
synergy of NLP, prompt engineering, and visual storytelling in making financial data more
accessible. Key limitations include lack of visual PDF parsing, restricted automation, and
infrastructure bottlenecks.
Looking ahead, future enhancements will focus on infrastructure scaling, automated chart
generation, multimodal document understanding, and prompt optimization tailored to financial
domains. This project serves as a compelling proof of concept for how generative AI can
democratize financial literacy, reduce analysis time, and enhance decision-making across
sectors.
