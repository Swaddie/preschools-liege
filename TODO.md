# TODO — Сайт пре-школ Льежа

> Файл для передачи контекста между чатами с Claude.
> Обновляй статусы по мере выполнения.

---

## Как начать новый чат

```
Продолжаем доделывать сайт с подборкой пре-школ Льежа.
— Репозиторий: https://github.com/Swaddie/preschools-liege
— Сайт: https://swaddie.github.io/preschools-liege/
— GitHub токен: YOUR_GITHUB_TOKEN

Склонируй репо, прочитай TODO.md и продолжим.
```

---

## Карточки: статус галерей и соцсетей

### ✅ Готово (галерея + Facebook)
- Les Deux Chênes — Modave
- Jardin Waldorf — Ferme Larock
- UWC Maastricht
- École de la Jeunesse — Seraing
- Institut Saint Maur — Cointe
- Sainte-Véronique Maternelle
- Notre-Dame de Méhagne — Embourg
- École du Haut — Fléron
- École libre de Préalle-Bas — Herstal
- École Libre des Monts — Herstal
- École Bellenay — Herstal
- EFLS Saint-Lambert — Saint-Nicolas ✅ (FB + галерея добавлены 16.05.2026)
- École Sainte-Thérèse — Seraing
- École Saint-Joseph — Seraing
- La Belle-Jardinière (Montessori) — Facebook есть
- École Montessori des Étoiles — Facebook + Instagram есть
- École fondamentale du Sartay — Embourg — Facebook есть
- Saint Louis de Gonzague — Flémalle — Facebook есть
- École de la Providence — Verviers — Facebook есть
- École Saint-Joseph (Grâce-Hollogne) — Facebook есть
- Jacques Brel — Herstal — Facebook есть

### 🖼️ Нужна галерея (нет фото)
- [ ] La Belle-Jardinière (Montessori) — Angleur
- [ ] École Montessori des Étoiles — Chênée
- [ ] School Saint Hubert — Saint-Nicolas
- [ ] Saint Louis de Gonzague — Flémalle
- [ ] École fondamentale du Sartay — Embourg
- [ ] École Princesse de Liège — Chaudfontaine
- [ ] École Libre de Theux
- [ ] École de la Providence — Verviers
- [ ] École Sinibaldo Basile
- [ ] École de Bierset — Immersion NL
- [ ] École Georges Simenon
- [ ] École des Champs
- [ ] École Julie et Mélissa
- [ ] École Saint-Étienne
- [ ] École Saint-Joseph (Grâce-Hollogne)
- [ ] École Sainte-Thérèse (Grâce-Hollogne)
- [ ] École communale de Loncin
- [ ] École communale d'Awans
- [ ] Écoles libres d'Awans
- [ ] École communale du Gros-Chêne
- [ ] École communale Jean-Marie Léonard
- [ ] École sportive Régis Genaux
- [ ] École Joseph Distexhe — Immersion NL
- [ ] École Jacques Brel — Herstal

### 📘 Нужен Facebook (не найден)
- [ ] École Montessori de Tilff
- [ ] School Saint Hubert — Saint-Nicolas
- [ ] Sainte-Marie de Boirs — Bassenge
- [ ] École Saint Dominique — Saint-Nicolas
- [ ] Enfant Jésus — Juprelle
- [ ] École Princesse de Liège — Chaudfontaine
- [ ] École Libre de Theux
- [ ] École Sinibaldo Basile
- [ ] École de Bierset — Immersion NL
- [ ] École Georges Simenon
- [ ] École des Champs
- [ ] École Julie et Mélissa
- [ ] École Saint-Étienne
- [ ] École Sainte-Thérèse (Grâce-Hollogne)
- [ ] École communale de Loncin
- [ ] École communale d'Awans
- [ ] Écoles libres d'Awans
- [ ] École communale du Gros-Chêne
- [ ] École communale Jean-Marie Léonard
- [ ] École sportive Régis Genaux
- [ ] École Joseph Distexhe — Immersion NL

---

## Другие задачи
- [ ] ...допиши сюда если есть другие идеи...

---

## Как добавить галерею (паттерн)

1. Найти карточку школы в `index.html`
2. Изменить `class="card"` → `class="card card-with-gallery"`
3. Заменить `<div class="card-body">` на блок с галереей:

```html
<div class="card-body-wrap">
  <div class="card-gallery">
    <div class="gallery-main">
      <img src="URL1" alt="описание" loading="lazy">
    </div>
    <div class="gallery-thumbs">
      <img src="URL2" alt="описание" loading="lazy">
      <img src="URL3" alt="описание" loading="lazy">
      ...
    </div>
  </div>
  <div class="card-body">
    <!-- строки адрес/язык/телефон -->
  </div>
</div>
```

4. Добавить кнопку Facebook в `card-links` если есть:
```html
<a class="link-btn" href="https://www.facebook.com/PAGE/" target="_blank">📘 Facebook</a>
```

5. Сделать `git add index.html && git commit -m "Название: галерея + FB" && git push`
