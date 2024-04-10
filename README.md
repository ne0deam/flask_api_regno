# flask_api_regno
**Развертывание системы**

git clone https://github.com/vavasya/Flask_API_ML_classify.git

cd Flask_API_ML_classify

docker-compose up -d

**Для примера можно кинуть тестовый POST запрос**
```
curl -L -X POST 'localhost:5000/reg/' \
-H 'Content-Type: application/json' \
-H 'x-api-key: 123321' \
--data-raw '{
  "regno_recognize": "А939НО196",
  "afts_regno_ai": "А939НО190",
  "recognition_accuracy": 6.4,
  "afts_regno_ai_score": 0.8689166903495789,
  "afts_regno_ai_char_scores": "[0.9998925924301147, 0.9999872446060181, 0.9999798536300659, 0.9999990463256836, 0.9988356232643127, 0.9998175501823425, 1.0, 0.999994158744812, 0.8702163696289062]",
  "afts_regno_ai_length_scores": "[3.2404470773350624e-10, 3.236617363011618e-10, 3.2367283853140805e-10, 3.2651523151905337e-10, 3.234087164738497e-10, 3.259402747701756e-10, 3.2362224011706076e-10, 4.545459564297971e-09, 2.996458192683349e-08, 1.0, 3.2479344214131345e-10]",
  "camera_type": "Стационарная",
  "camera_class": "Астра-Трафик",
  "time_check": "2021-08-01 09:02:59",
  "direction": 0
}'
```
