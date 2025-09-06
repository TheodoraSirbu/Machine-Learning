📌 Descriere proiect

Proiectul urmărește clasificarea imaginilor de fluturi utilizând atât metode tradiționale de învățare automată, cât și rețele neuronale convoluționale (CNN), incluzând un model construit de la zero și un model pre-antrenat (MobileNetV2).

📂 Împărțirea setului de date

Setul de date a fost împărțit în 80% pentru antrenare, 10% pentru validare și 10% pentru testare, folosind stratificarea pentru păstrarea proporțiilor claselor. Încărcarea și augmentarea datelor s-au realizat prin ImageDataGenerator.

⚙️ Prelucrarea datelor

Imaginile au fost redimensionate la dimensiuni standard (180x180 sau 224x224 pixeli). S-au aplicat tehnici de augmentare, precum rotații, zoom și flip orizontal. Pentru MobileNetV2 s-a utilizat și funcția de preprocesare specifică modelului.

🤖 Metode folosite

🔹	CNN construit de la zero – rețea cu straturi convoluționale, pooling, normalizare și dense.

🔹	Random Forest – antrenat pe vectori de caracteristici extrase din imagini.

🔹 CNN pre-antrenat (MobileNetV2) – folosit ca extractor de caracteristici și ajustat prin fine-tuning.

📊 Rezultate

Performanța modelelor pe setul de test a fost următoarea:

🔹 CNN Simplu – acuratețe de 73%

🔹 Random Forest – acuratețe de 31%

🔹 CNN pre-antrenat (MobileNetV2) – acuratețe de 88%

Modelul MobileNetV2 a obținut cele mai bune rezultate, confirmând eficiența utilizării transfer learning-ului în clasificarea imaginilor.