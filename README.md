[![Tests](https://github.com/DancheG14/devops_project/actions/workflows/docker-image.yml/badge.svg)](https://github.com/DancheG14/devops_project/actions/workflows/docker-image.yml)

#                                                           **devops_project**  

##                             Учебный проект по дисциплине "Распределённые и параллельные вычисления"  

### В данном проекте выполнено создание  управляемого кластера Kubernetes в Яндекс.Облаке и развертывание в нем двух связанных контейнеров приложения распознавания токсичности текста.   В одном контейнере, реализованом через FastAPI и сервис Uvicorn, происходит загрузка предобученной модели-трансформера *[lordtt13/emo-mobilebert](https://huggingface.co/lordtt13/emo-mobilebert?text=I+like+you.+I+love+you)*, приём в виде ***json*** введённого во втором контейнера приложения текста, на вход модели и распознавание, с последующей передачей результата в виде двух аргументов ***json***( вероятности в процентах и степени токсичности  текста) обратно во второй контейнер, реализованном в виде web-приложения сервиса Streamlit
