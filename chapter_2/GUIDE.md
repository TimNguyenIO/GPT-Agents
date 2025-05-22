# Chapter 2: File Guide

This guide provides an overview of the main Python files in this chapter, including their purpose, usage, and learning outcomes.

---

## 1. connecting.py
**Introduction:**
Handles connecting to the OpenAI API, loading API keys securely, and sending prompts to ChatGPT.

**Why:**
Demonstrates secure API usage and basic interaction with GPT models.

**How to Run/Test:**
- Ensure your `.env` file contains your OpenAI API key.
- Run: `python connecting.py`
- The script will print a response from ChatGPT.

**What to Learn:**
- How to securely load API keys
- How to send and receive messages with OpenAI's API

---

## 2. json_output.py
**Introduction:**
Handles formatting and parsing JSON output from model responses.

**Why:**
Many AI models return or require JSON for structured data exchange.

**How to Run/Test:**
- Run: `python json_output.py`

**What to Learn:**
- How to parse, validate, and format JSON in Python.

---

## 3. lmstudio_server.py
**Introduction:**
Provides a local server interface for interacting with language models.

**Why:**
Useful for local development, testing, or integrating with other tools.

**How to Run/Test:**
- Download and install LM Studio from [https://lmstudio.ai/](https://lmstudio.ai/)
- Start LM Studio locally:
  - On macOS, open the Applications folder and double-click **LM Studio**
  - Or run from terminal:
    ```bash
    open -a "LM Studio"
    ```
- Click on Developer icon on the left then click on Start Server
- Run: `python lmstudio_server.py`

**What to Learn:**
- How to set up a local server for model inference.

---

## 4. message_history.py
**Introduction:**
Manages conversation or message history for chat-based applications.

**Why:**
Maintaining message history is crucial for context-aware AI interactions.

**How to Run/Test:**
- Run: `python message_history.py`

**What to Learn:**
- How to store, retrieve, and manage message history in Python.

---

## 5. prompt_engineering.py
**Introduction:**
Contains utilities and examples for crafting effective prompts for language models.

**Why:**
Good prompt engineering improves model performance and output quality.

**How to Run/Test:**
- Run: `python prompt_engineering.py`

**What to Learn:**
- Techniques for prompt design and evaluation.

---

## 6. prompt_utils.py
**Introduction:**
Provides helper functions for prompt formatting, validation, or manipulation.

**Why:**
Reusable utilities streamline prompt creation and reduce errors.

**How to Run/Test:**
- Run: `python prompt_utils.py`

**What to Learn:**
- How to build and use prompt utility functions in Python.

---

# Glossary (Giải thích thuật ngữ)

- **API key**: Khóa truy cập dùng để xác thực khi kết nối tới dịch vụ OpenAI. (Mã bí mật để xác thực ứng dụng của bạn với OpenAI)
- **Environment variable (.env)**: Biến môi trường, thường lưu thông tin nhạy cảm như API key, cấu hình, v.v. (Biến môi trường giúp bảo mật thông tin cấu hình)
- **Virtual environment (venv)**: Môi trường Python ảo, giúp cô lập các thư viện cho từng dự án. (Mỗi dự án có thể dùng phiên bản thư viện riêng)
- **Prompt**: Đoạn văn bản đầu vào gửi cho mô hình AI để nhận kết quả mong muốn. (Câu hỏi hoặc hướng dẫn gửi cho AI)
- **Prompt engineering**: Kỹ thuật thiết kế prompt để tối ưu kết quả từ mô hình AI. (Cách viết prompt hiệu quả)
- **LM Studio**: Ứng dụng giúp chạy và thử nghiệm các mô hình ngôn ngữ lớn (LLM) trên máy tính cá nhân. (Phần mềm hỗ trợ làm việc với AI offline)
- **Message history**: Lịch sử hội thoại, lưu lại các tin nhắn giữa người dùng và AI. (Lưu lại nội dung trao đổi để AI hiểu ngữ cảnh)
- **Server**: Máy chủ, nơi chạy các dịch vụ hoặc mô hình AI để nhận và trả lời yêu cầu từ client. (Máy tính phục vụ xử lý trung tâm)
- **Generative models**: Mô hình sinh dữ liệu mới dựa trên dữ liệu đã học, ví dụ như tạo văn bản, hình ảnh, âm thanh. (AI có thể "sáng tạo" nội dung mới)
- **Large Language Model (LLMs)**: Mô hình ngôn ngữ lớn, được huấn luyện trên lượng dữ liệu văn bản khổng lồ để hiểu và sinh ngôn ngữ tự nhiên. (AI hiểu và tạo ra văn bản giống con người)
- **Generative Pretrained Transformers (GPTs)**: Dòng mô hình AI dựa trên kiến trúc Transformer, được huấn luyện trước để sinh ngôn ngữ tự nhiên. (GPT là ví dụ nổi bật của LLM)
- **Fine Tuning**: Quá trình tinh chỉnh mô hình AI trên tập dữ liệu nhỏ, chuyên biệt để cải thiện hiệu suất cho tác vụ cụ thể. (Huấn luyện thêm để AI phù hợp hơn với nhu cầu riêng)
- **Reinforcement learning with human feedback (RLHF)**: Học tăng cường với phản hồi từ con người, giúp AI học cách trả lời tốt hơn dựa trên đánh giá của người dùng. (AI học từ phản hồi thực tế của con người)
- **Messages**: Các tin nhắn trao đổi giữa người dùng và AI trong một phiên hội thoại. (Thông điệp gửi/nhận giữa người và AI)
- **User role**: Vai trò người dùng, đại diện cho các yêu cầu hoặc câu hỏi gửi tới AI. (Người sử dụng AI)
- **System role**: Vai trò hệ thống, dùng để thiết lập bối cảnh hoặc hướng dẫn cho AI trước khi hội thoại bắt đầu. (Thiết lập ngữ cảnh, quy tắc cho AI)
- **Assistant role**: Vai trò trợ lý, đại diện cho phản hồi của AI đối với người dùng. (AI trả lời hoặc hỗ trợ người dùng)
- **Prompt Engineering Strategies**: Các chiến lược thiết kế prompt giúp AI hiểu và trả lời tốt hơn.
    1. **Write Clear Instructions (Basic)**: Viết hướng dẫn rõ ràng, cụ thể để AI dễ hiểu và thực hiện đúng yêu cầu.
        - *Ví dụ*: "Hãy liệt kê 3 thành phố lớn nhất ở Việt Nam."
    2. **Provide Reference Text (Memory)**: Cung cấp đoạn văn bản tham khảo để AI dựa vào đó trả lời chính xác hơn.
        - *Ví dụ*: "Dựa vào đoạn sau: 'Hà Nội là thủ đô, TP.HCM là thành phố lớn nhất', hãy cho biết thủ đô Việt Nam là gì?"
    3. **Use External Tools (Memory)**: Kết hợp AI với công cụ ngoài (như tìm kiếm, cơ sở dữ liệu) để bổ sung trí nhớ hoặc thông tin.
        - *Ví dụ*: "Hãy tra cứu Wikipedia và cho biết năm thành lập Đại học Quốc gia Hà Nội."
    4. **Split Complex Tasks into Simple Subtasks (Planning)**: Chia bài toán lớn thành các bước nhỏ, đơn giản để AI giải quyết từng phần.
        - *Ví dụ*: "Bước 1: Tính tổng số học sinh. Bước 2: Tính số học sinh giỏi. Bước 3: Tính tỷ lệ học sinh giỏi."
    5. **Give Models Time to Think (Planning)**: Yêu cầu AI giải thích hoặc suy nghĩ từng bước trước khi trả lời cuối cùng.
        - *Ví dụ*: "Hãy giải thích từng bước cách giải bài toán này trước khi đưa ra đáp án."
    6. **Test Changes Systematically (Evaluation)**: Thay đổi prompt và kiểm tra kết quả một cách có hệ thống để đánh giá hiệu quả.
        - *Ví dụ*: "Thử thay đổi câu hỏi từ 'Kể tên' sang 'Liệt kê' và so sánh kết quả trả lời của AI."
- **Quality Criteria khi sử dụng LLMs**: Các tiêu chí đánh giá chất lượng khi lựa chọn và sử dụng mô hình ngôn ngữ lớn.
    1. **Model Parameters (Size)**: Số lượng tham số của mô hình, mô hình càng lớn thường càng mạnh nhưng tốn tài nguyên hơn.
        - *Ví dụ*: GPT-3 có 175 tỷ tham số, GPT-2 chỉ có 1,5 tỷ tham số.
    2. **Model Performance**: Hiệu suất của mô hình trên các tác vụ thực tế (độ chính xác, khả năng hiểu ngữ cảnh, v.v.).
        - *Ví dụ*: Mô hình trả lời đúng 9/10 câu hỏi về lịch sử.
    3. **Model Cost (Project Budget)**: Chi phí sử dụng mô hình, bao gồm phí API, chi phí hạ tầng, v.v.
        - *Ví dụ*: Sử dụng GPT-4 tốn nhiều tiền hơn GPT-3.5 cho cùng một lượng câu hỏi.
    4. **Model Speed (Model Deployment)**: Tốc độ phản hồi của mô hình khi triển khai thực tế.
        - *Ví dụ*: GPT-3.5 trả lời trong 2 giây, GPT-4 mất 5 giây cho cùng một câu hỏi.
    5. **Context token Size**: Số lượng token (ký tự, từ) mà mô hình có thể xử lý trong một lần.
        - *Ví dụ*: GPT-3.5 hỗ trợ 4.096 token, GPT-4 hỗ trợ 32.000 token (có thể xử lý văn bản dài hơn).
    6. **Training Method**: Phương pháp huấn luyện mô hình (huấn luyện trước, tinh chỉnh, RLHF, v.v.).
        - *Ví dụ*: GPT-4 được huấn luyện bằng RLHF để cải thiện chất lượng trả lời.
    7. **Training Input**: Dữ liệu đầu vào dùng để huấn luyện mô hình (sách, báo, website, v.v.).
        - *Ví dụ*: Mô hình được huấn luyện trên dữ liệu Wikipedia, sách tiếng Anh, và các trang web phổ biến.
