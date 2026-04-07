FROM python:3.10-slim

WORKDIR /app

# Install dependencies
RUN pip install --no-cache-dir django==3.2

# Copy project
COPY . .

# Expose port
EXPOSE 8000

# Run migrations at container startup (NOT build time)
CMD ["sh", "-c", "python manage.py migrate && python manage.py runserver 0.0.0.0:8000"]