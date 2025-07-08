# Все Техники RAG: Простой, Практический Подход ✨

Read this in your preferred language:  
[Deutsch](https://www.readme-i18n.com/FareedKhan-dev/all-rag-techniques?lang=de) |  [Español](https://www.readme-i18n.com/FareedKhan-dev/all-rag-techniques?lang=es) |  [Français](https://www.readme-i18n.com/FareedKhan-dev/all-rag-techniques?lang=fr) |  [日本語](https://www.readme-i18n.com/FareedKhan-dev/all-rag-techniques?lang=ja) |  [한국어](https://www.readme-i18n.com/FareedKhan-dev/all-rag-techniques?lang=ko) |  [Português](https://www.readme-i18n.com/FareedKhan-dev/all-rag-techniques?lang=pt) | [Русский](https://www.readme-i18n.com/FareedKhan-dev/all-rag-techniques?lang=ru) |  [中文](https://www.readme-i18n.com/FareedKhan-dev/all-rag-techniques?lang=zh)

[![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/) [![Nebius AI](https://img.shields.io/badge/Nebius%20AI-API-brightgreen)](https://cloud.nebius.ai/services/llm-embedding) [![OpenAI](https://img.shields.io/badge/OpenAI-API-lightgrey)](https://openai.com/) [![Medium](https://img.shields.io/badge/Medium-Blog-black?logo=medium)](https://medium.com/@fareedkhandev/testing-every-rag-technique-to-find-the-best-094d166af27f)

Это хранилище использует четкий, практический подход к **Retrieval-Augmented Generation (RAG)**, разбивая передовые методы на простые, понятные реализации. Вместо того, чтобы полагаться на такие рамки, как `LangChain` or `FAISS`, все здесь построено с использованием знакомых библиотек Python `openai`, `numpy`, `matplotlib`, и несколько других.

Цель проста: создать код, который был бы удобочитаемым, модифицируемым и образовательным. Уделяя особое внимание основам, этот проект помогает развеять мистификацию RAG и облегчает понимание того, как он работает на самом деле.

## Update: 📢

- (12-May-2025) Added a new notebook on how to handle big data using Knowledge Graphs.
- (27-April-2025) Added a new notebook which finds best RAG technique for a given query (Simple RAG + Reranker + Query Rewrite).
- (20-Mar-2025) Added a new notebook on RAG with Reinforcement Learning.
- (07-Mar-2025) Added 20 RAG techniques to the repository.

## 🚀 What's Inside?

Этот репозиторий содержит коллекцию записных Jupyter Notebooks, каждая из которых посвящена определенной технике RAG.  Каждая Notebooks содержит:

- Краткое объяснение техники.
- Пошаговую реализацию с нуля.
- Понятные примеры кода со встроенными комментариями.
- Оценки и сравнения для демонстрации эффективности методики.
- Визуализация для наглядного представления результатов.

Вот краткий обзор рассмотренных методик:

| Notebook                                      | Description                                                                                                                                                         |
| :-------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [1. Simple RAG](01_simple_rag.ipynb)           | Базовая реализация RAG.  Отличная отправная точка!                                                                                                      |
| [2. Semantic Chunking](02_semantic_chunking.ipynb) | Разбивает текст на основе семантического сходства на более значимые фрагменты.                                                                                          |
| [3. Chunk Size Selector](03_chunk_size_selector.ipynb) | Исследуется влияние различных размеров фрагментов на производительность поиска.                                                                                    |
| [4. Context Enriched RAG](04_context_enriched_rag.ipynb) | Извлекает соседние фрагменты, чтобы предоставить больше контекста.                                                                                                     |
| [5. Contextual Chunk Headers](05_contextual_chunk_headers_rag.ipynb) | Добавляет описательные заголовки к каждому фрагменту перед внедрением.                                                                                                |
| [6. Document Augmentation RAG](06_doc_augmentation_rag.ipynb) | Генерирует вопросы из фрагментов текста, чтобы ускорить процесс поиска.                                                                                           |
| [7. Query Transform](07_query_transform.ipynb)   | Переписывает, расширяет или декомпозирует запросы для улучшения поиска.  Включает в себя ** Пошаговый запрос ** и ** Декомпозицию подзапросов**.                                      |
| [8. Reranker](08_reranker.ipynb)               | Повторно ранжирует первоначально полученные результаты с помощью LLM для повышения их релевантности.                                                                                       |
| [9. RSE](09_rse.ipynb)                         | Извлечение релевантных сегментов:  Идентифицирует и реконструирует непрерывные сегменты текста, сохраняя контекст.                                                  |
| [10. Contextual Compression](10_contextual_compression.ipynb) | Реализует контекстуальное сжатие для фильтрации и сжатия извлеченных фрагментов, максимизируя релевантную информацию.                                                |
| [11. Feedback Loop RAG](11_feedback_loop_rag.ipynb) | Учитывает отзывы пользователей для изучения и совершенствования системы RAG с течением времени.                                                                                      |
| [12. Adaptive RAG](12_adaptive_rag.ipynb)     | Динамически выбирает наилучшую стратегию поиска в зависимости от типа запроса.                                                                                         |
| [13. Self RAG](13_self_rag.ipynb)             | Реализует SelfRAG, динамически решает, когда и как извлекать данные, оценивает релевантность, а также поддержку и полезность.                                        |
| [14. Proposition Chunking](14_proposition_chunking.ipynb) | Разбивает документы на атомарные, фактические утверждения для точного поиска.                                                                                      |
| [15. Multimodel RAG](15_multimodel_rag.ipynb)   | Объединяет текст и изображения для поиска, создавая подписи к изображениям с помощью Lava.                                                                  |
| [16. Fusion RAG](16_fusion_rag.ipynb)         | Сочетает векторный поиск с поиском по ключевым словам (BM25) для улучшения результатов.                                                                                |
| [17. Graph RAG](17_graph_rag.ipynb)           | Упорядочивает знания в виде графа, позволяя просматривать связанные понятия.                                                                                        |
| [18. Hierarchy RAG](18_hierarchy_rag.ipynb)        | Создает иерархические индексы (сводки + подробные фрагменты) для эффективного поиска.                                                                                   |
| [19. HyDE RAG](19_HyDE_rag.ipynb)             | Использует вложения в гипотетические документы для улучшения семантического соответствия.                                                                                              |
| [20. CRAG](20_crag.ipynb)                     | Корректирующий RAG: динамически оценивает качество поиска и использует веб-поиск в качестве запасного варианта.                                                                           |
| [21. Rag with RL](21_rag_with_rl.ipynb)                     | Максимизируйте вознаграждение за модель RAG, используя обучение с подкреплением.                                                                           |
| [Best RAG Finder](best_rag_finder.ipynb)     | Находит наилучший метод RAG для данного запроса, используя простой RAG + Reranker + Rewrite запроса.                                                                        |
| [22. Big Data with Knowledge Graphs](22_Big_data_with_KG.ipynb) | Обрабатывает большие наборы данных с помощью графов знаний.                                                                                                                     |

## 🗂️ Repository Structure

```
fareedkhan-dev-all-rag-techniques/
├── README.md                          <- You are here!
├── 01_simple_rag.ipynb
├── 02_semantic_chunking.ipynb
├── 03_chunk_size_selector.ipynb
├── 04_context_enriched_rag.ipynb
├── 05_contextual_chunk_headers_rag.ipynb
├── 06_doc_augmentation_rag.ipynb
├── 07_query_transform.ipynb
├── 08_reranker.ipynb
├── 09_rse.ipynb
├── 10_contextual_compression.ipynb
├── 11_feedback_loop_rag.ipynb
├── 12_adaptive_rag.ipynb
├── 13_self_rag.ipynb
├── 14_proposition_chunking.ipynb
├── 15_multimodel_rag.ipynb
├── 16_fusion_rag.ipynb
├── 17_graph_rag.ipynb
├── 18_hierarchy_rag.ipynb
├── 19_HyDE_rag.ipynb
├── 20_crag.ipynb
├── 21_rag_with_rl.ipynb
├── 22_big_data_with_KG.ipynb
├── best_rag_finder.ipynb
├── requirements.txt                   <- Python dependencies
└── data/
    └── val.json                       <- Sample validation data (queries and answers)
    └── AI_Information.pdf             <- A sample PDF document for testing.
    └── attention_is_all_you_need.pdf  <- A sample PDF document for testing (for Multi-Modal RAG).
```

## 🛠️ Getting Started

1. **Clone the repository:**

    ```bash
    git clone https://github.com/FareedKhan-dev/all-rag-techniques.git
    cd all-rag-techniques
    ```

2. **Install dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

3. **Set up your OpenAI API key:**

    - Obtain an API key from [Nebius AI](https://studio.nebius.com/).
    - Set the API key as an environment variable:

        ```bash
        export OPENAI_API_KEY='YOUR_NEBIUS_AI_API_KEY'
        ```

        or

        ```bash
        setx OPENAI_API_KEY "YOUR_NEBIUS_AI_API_KEY"  # On Windows
        ```

        or, within your Python script/notebook:

        ```python
        import os
        os.environ["OPENAI_API_KEY"] = "YOUR_NEBIUS_AI_API_KEY"
        ```

4. **Run the notebooks:**

    Откройте любой из блокнотов Jupyter (файлы `.ipynb`) с помощью Jupyter Notebook или JupyterLab.  Каждый блокнот является автономным и может запускаться независимо.  Блокноты предназначены для последовательного запуска в каждом файле.

    **Примечание:** Файл `data/AI_Information.pdf` содержит образец документа для тестирования. Вы можете заменить его своим собственным PDF-файлом.  Файл `data/val.json` содержит примеры запросов и идеальные ответы для оценки.
    Файл "attention_is_all_you_need.pdf" предназначен для тестирования мультимодального блокнота RAG.

## 💡 Основные концепции

- ** Embeddings: ** Числовое представление текста, которое отражает семантический смысл.  Мы используем API для встраивания Nebius AI и, во многих ноутбуках, также модель встраивания "BAAI/bge-en-icl".

- **Хранилище векторов: Vector Store:** Простая база данных для хранения и поиска вложений.  Мы создаем наш собственный класс SimpleVectorStore, используя NumPy для эффективного вычисления подобия.

- **Косинусное сходство: Cosine Similarity:** Мера сходства между двумя векторами.  Более высокие значения указывают на большее сходство.

- ** Разбиение текста на фрагменты: Chunking:** Разделение текста на более мелкие, удобные для восприятия фрагменты.  Мы изучаем различные стратегии разбиения текста на фрагменты.

- **Извлечение: Retrieval:** Процесс поиска наиболее релевантных фрагментов текста для данного запроса.

- **Генерация: Generation:** Использование большой языковой модели (LLM) для создания ответа на основе полученного контекста и запроса пользователя.  Мы используем модель "meta-llama/Llama-3.2-3B-Instruct" через API Nebius AI.

- **Оценка: Evaluation:** Оценка качества ответов системы RAG, часто путем сравнения их с эталонными ответами или с помощью LLM для оценки значимости.

## 🤝 Внесение вклада

Приветствуются вклады!
