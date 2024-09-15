# Gunakan `python:3.11.4` sebagai base image
FROM python:3.11.4

# Set workdir di dalam kontainer
WORKDIR /app

# Copy Requirements file ke dalam kontainer
COPY requirements.txt .

# Install seluruh libraries yang dibutuhkan
RUN pip install --no-cache-dir -r requirements.txt

# Copy seluruh kode yang ada pada folder etl
COPY . .

# Ekspose port API
EXPOSE 6000

# Mendefiniskan command
CMD ["python", "api.py"]
