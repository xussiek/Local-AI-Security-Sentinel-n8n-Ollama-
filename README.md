# Local-AI-Security-Sentinel-n8n-Ollama-
Automatyczny system monitorowania zagrożeń cyberbezpieczeństwa, który pobiera dane z polskich i światowych serwisów security, analizuje je lokalnie przy użyciu modelu LLM (Mistral/Llama 3) i przesyła techniczne podsumowania na Discorda.
Główne Funkcje
Multi-Source Aggregation: Łączy dane z RSS (Niebezpiecznik, Sekurak, Zaufana Trzecia Strona).

Custom Data Parser: Autorski skrypt JavaScript czyszczący surowy tekst z reklam, tagów HTML i spamu RODO (oszczędność tokenów).

Privacy-First AI: Analiza odbywa się w 100% lokalnie na modelu Mistral 7B (via Ollama), co gwarantuje, że dane nie opuszczają Twojej maszyny.

Smart Batching: System przetwarza artykuły sekwencyjnie, optymalizując zużycie VRAM (testowane na RTX 3060 12GB).

Discord Integration: Wyniki trafiają na dedykowany kanał w formie czytelnych raportów technicznych.

🛠️ Stack Techniczny
n8n: Orchestracja workflow.

Ollama: Silnik do uruchamiania lokalnych modeli LLM.

JavaScript: Zaawansowane parsowanie i transformacja danych.

Discord Webhooks: Kanał komunikacji.

📦 Jak uruchomić?
Zainstaluj i uruchom Ollamę (ollama pull mistral).

Zaimportuj plik .json do swojego n8n.

Skonfiguruj Variables w n8n lub podepnij własny Discord Webhook URL.

(Opcjonalnie) Ustaw Schedule Trigger, aby system działał automatycznie co X godzin.
