# 📚 Атлас треков HackAlem AI: Вайб-кодинг и архитектура победителей

Полная база знаний по всем 12 трекам крупнейшего международного AI-хакатона **HackAlem AI** (Астана, рекорд Guinness). В каждом документе детально разобраны проекты команд 1–3 мест, их технологический стек, структура файлов, git-ветки, координация ИИ-агентов и киллер-фичи перед жюри.

---

## 🗺 Навигация по всем 12 трекам

| № | Трек | Кейс-партнер | Ключевой стек победителей | Документ с полным разбором |
| :-: | :--- | :--- | :--- | :--- |
| **01** | **Телекоммуникации** | Beeline | Python, SciPy (HiGHS MILP), React + Tauri, Bayes, OpenAI | [Разбор трека 01](track_01_telecom.md) |
| **02** | **Финансы** | Freedom / Halyk | Next.js 16, TypeScript, Sigma.js, Parquet, gpt-6-luna | [Разбор трека 02](track_02_finance.md) |
| **03** | **Логистика и закупки** | Электрокомплект | Vercel PWA, Django, FastAPI, Hampel Filter, WhatsApp/TG API | [Разбор трека 03](track_03_logistics.md) |
| **04** | **Торговля** | ekt.kz | Next.js 16, React 19, Tailwind 4, Multimodal Vision, Zod | [Разбор трека 04](track_04_retail.md) |
| **05** | **Инновации** | «Хаттама» (Госсектор) | vLLM, RTX 6000, SeamlessM4T-v2, Apple MLX, NeMo, Gemma | [Разбор трека 05](track_05_innovations.md) |
| **06** | **Энергетика** | Самрук-Казына | LightGBM, scikit-learn, Streamlit, DuckDB, Three.js 3D | [Разбор трека 06](track_06_energy.md) |
| **07** | **Коммуникации** | Halyk (Voice Router) | Next.js 16, WebRTC (живой перехват), Go, ESPnet, Neon DB | [Разбор трека 07](track_07_communications.md) |
| **08** | **Образование** | Challenge Hub | FastAPI, uv, Go, PostgreSQL SKIP LOCKED, Playwright | [Разбор трека 08](track_08_education.md) |
| **09** | **Управление** | Career Quest | React 19, better-sqlite3, Go, Django DRF, Zero-PII | [Разбор трека 09](track_09_management.md) |
| **10** | **Креативные индустрии** | #79-lite (Подрядчики) | FastAPI, text-embedding-3-large, Reason Codes, shadcn/ui | [Разбор трека 10](track_10_creative.md) |
| **11** | **Astana Innovations** | «Аким на 5 часов» | Next.js 16, Mapbox/Leaflet, Quality of Life Score, 0-Dep | [Разбор трека 11](track_11_astana.md) |
| **12** | **Казахтелеком** | Сравнение оргструктур | Bun, Next.js 16, React Flow, ONNX Runtime, adilet.zan.kz | [Разбор трека 12](track_12_kazakhtelecom.md) |

---

## 💎 Главные паттерны вайб-кодинга победителей (The Golden Vibe-Coding Rules):

1. **Разделение ролей ИИ (`AGENTS.md`):**  
   Один агент пишет математику и алгоритмы (Claude Opus), второй агент пишет интерфейс и проводит независимый аудит (ChatGPT / Codex).
2. **«The Gate» перед коммитом:**  
   Никакого мусора в репозитории — жесткая проверка линтером, типами и тестами (`pnpm check` или `pytest`).
3. **Строгий барьер для LLM (No Hallucinations):**  
   Языковая модель **никогда не считает деньги и не принимает окончательных решений**. Логику, фильтрацию и скоринг считает детерминированный код (Python / Go / TypeScript), а LLM лишь формулирует человекочитаемое объяснение (Reason Codes).
4. **Offline / Mock Mode для жюри:**  
   Возможность запустить проект за 10 секунд без ввода API-ключей спасает от падений перегруженного Wi-Fi на хакатоне.
5. **Визуализация важнее чистого JSON:**  
   Проекты с интерактивными графами (**Sigma.js**), деревьями оргструктур (**React Flow**), картами (**Mapbox**) и 3D-графикой (**Three.js**) побеждают скучные текстовые консоли в 10 случаях из 10.
