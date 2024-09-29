FROM python:3.9.20-slim

WORKDIR /usr/src/app

COPY ./requirements.txt .
 
# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the code
COPY . .
EXPOSE 8001

CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8001"]
