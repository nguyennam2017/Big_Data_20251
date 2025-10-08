Chỉ dẫn nhanh để chạy `crawl/crawl.py` bằng Poetry (Windows PowerShell)

1) Cài Poetry (nếu chưa có). Chạy trong PowerShell (chạy như Administrator nếu gặp lỗi):

   (Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | py -

   Sau khi cài, khởi động lại PowerShell hoặc chạy `RefreshEnv` / mở cửa sổ mới.

2) Tạo virtualenv và cài dependency từ `pyproject.toml`:

   poetry install

   (Nếu muốn một virtualenv cụ thể: `poetry env use C:\path\to\python.exe` trước khi `poetry install`)

3) Chạy script crawl trong môi trường Poetry:

   poetry run python crawl\crawl.py
