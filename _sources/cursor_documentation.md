# NEUROML Course - Техническая документация

## Описание проекта

**Название:** Neuroimaging and Machine Learning for Biomedicine  
**Авторы:** Nadezhda Alsahanova, Aleksandra Beliaeva  
**Организация:** Skoltech BIMAI Lab  

Курс по машинному обучению в анализе нейровизуализационных данных, включающий теоретический материал и практические семинары по работе с EEG, MRI, fMRI данными.

## Архитектура проекта

### Структура файлов

- `_config.yml` - конфигурация Jupyter Book
- `_toc.yml` - таблица содержания курса
- `requirements.txt` - зависимости Python
- `intro.md` - главная страница курса
- `seminar0/` - вводные материалы (Python, ML, PyTorch основы)
- `seminar1/` - работа с EEG данными
- `seminar2/` - MRI анализ (с Docker поддержкой)
- `seminar4/` - fMRI анализ и коннективность
- `bio/` - биологическая информация и ссылки

### Технический стек

- **Основа:** Jupyter Book для создания интерактивной документации
- **Python:** 3.13 (текущая версия в окружении)
- **Основные библиотеки:**
  - numpy, pandas, scipy, scikit-learn
  - matplotlib, seaborn - визуализация
  - nibabel, nilearn - нейровизуализация
  - mne - EEG анализ
  - nipype - нейропроцессинг пайплайны
  - antspyx, SimpleITK - обработка изображений

## Семинары

1. **Seminar 0** - Введение: Python, ML, PyTorch основы
2. **Seminar 1** - EEG анализ и машинное обучение
3. **Seminar 2-3** - MRI данные: базы данных, трансформации, FreeSurfer
4. **Seminar 4-6** - fMRI: препроцессинг, GLM, функциональные связи
5. **Seminar 7** - Интерпретация моделей машинного обучения

## Технические особенности

### Docker поддержка
- Семинары 2 и 4 используют Docker контейнеры
- Конфигурационные файлы: `Dockerfile`, `docker.md`

### Внешние ссылки
- Google Colab notebooks для некоторых семинаров
- YouTube лекции и Google Drive материалы
- Репозиторий: https://github.com/BIMAI-lab/NEUROML_course

## Проблемы и решения

### Текущие проблемы
1. **Конфликт зависимостей urllib3/six** - требует обновления requirements.txt
2. **Несовместимость с Python 3.13** - некоторые библиотеки требуют совместимые версии

### TODO
- [x] Создать техническую документацию
- [ ] Исправить конфликт зависимостей в requirements.txt
- [ ] Протестировать сборку Jupyter Book
- [ ] Добавить версионирование для всех зависимостей

## Команды для работы

### Активация окружения
```bash
source .venv/bin/activate  # или активация вашего виртуального окружения
```

### Сборка книги
```bash
jupyter-book build .
```

### Установка зависимостей
```bash
pip install -r requirements.txt
```

## Конфигурация Jupyter Book

- **Автоисполнение:** `execute_notebooks: force`
- **Тема:** стандартная с кастомным CSS (`_static/myadmonitions.css`)
- **Интеграция:** GitHub buttons, issues, repository links
- **Вывод:** HTML и LaTeX (NeuroML.tex)

## Данные и датасеты

- Human Connectome Project (HCP)
- EEG Motor Movement/Imagery Dataset
- ABIDE (Autism Brain Imaging Data Exchange)
- ADNI (Alzheimer Disease Neuroimaging Initiative)

*Примечание: Требуется регистрация и соглашение об использовании данных*
