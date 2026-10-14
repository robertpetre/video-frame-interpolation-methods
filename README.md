# Comparative Analysis of Video Frame Interpolation Methods

## 1. Descrierea proiectului

Proiectul isi propune studiul, implementarea si evaluarea comparativa a mai multor metode de interpolare a cadrelor video, cu scopul de a creste rata de cadre a unui videoclip prin generarea unor cadre intermediare.

Interpolarea video reprezinta procesul de estimare a unuia sau mai multor cadre inexistente intre doua cadre consecutive. Aceasta tehnologie poate fi utilizata pentru cresterea fluiditatii videoclipurilor, generarea efectelor slow-motion, restaurarea continutului video si imbunatatirea experientei vizuale.

Proiectul va analiza atat calitatea cadrelor generate, cat si performanta computationala a algoritmilor utilizati, urmarind identificarea avantajelor si limitarilor fiecarei abordari.

## 2. Obiective

- Studierea principalelor tehnici de interpolare a cadrelor video.
- Selectarea si integrarea mai multor algoritmi de interpolare.
- Dezvoltarea unei aplicatii demonstrative pentru procesarea videoclipurilor.
- Compararea calitatii cadrelor generate folosind metrici obiective.
- Evaluarea timpului de procesare si a cerintelor computationale.
- Analizarea comportamentului algoritmilor in scenarii cu miscare rapida, schimbari de perspectiva si ocluziuni.
- Identificarea situatiilor in care fiecare metoda ofera rezultate mai bune.

## 3. Metodologie propusa

Vor fi investigate atat metode clasice bazate pe estimarea miscarii (*Optical Flow*), cat si metode moderne bazate pe *Deep Learning*.

Printre algoritmii avuti in vedere se numara:

- **RIFE (Real-Time Intermediate Flow Estimation)**
- **AMT (All-Pairs Multi-Field Transforms)**
- **FILM (Frame Interpolation for Large Motion)**
- Alte metode relevante, in functie de rezultatele cercetarii si de fezabilitatea implementarii.

Selectia finala a algoritmilor va fi stabilita in etapa de cercetare.

Pentru evaluare, vor fi utilizate videoclipuri cu rata de cadre ridicata, din care vor fi eliminate periodic cadre pentru simularea unui videoclip cu FPS redus.

Algoritmii vor incerca reconstruirea cadrelor eliminate, iar rezultatele vor fi comparate cu imaginile originale.

## 4. Evaluarea performantei

Comparatia dintre metode va urmari mai multe criterii:

**Calitatea imaginii:**
- PSNR (Peak Signal-to-Noise Ratio)
- SSIM (Structural Similarity Index)
- LPIPS (Learned Perceptual Image Patch Similarity), daca este aplicabil

**Performanta computationala:**
- Timpul de procesare
- Numarul de cadre procesate pe secunda
- Consumul de resurse hardware, in functie de posibilitatile de masurare

**Evaluare vizuala:**
- Calitatea interpolarii in scene cu miscare rapida
- Artefacte vizuale si deformari ale obiectelor
- Comportamentul in cazul ocluziunilor si al schimbarilor bruste de scena

Testele vor urmari conditii comparabile pentru fiecare algoritm, utilizand aceleasi videoclipuri, rezolutii si configuratii hardware, acolo unde este posibil.

## 5. Aplicatia demonstrativa

Se urmareste dezvoltarea unei aplicatii care sa permita:

- Incarcarea unui videoclip.
- Selectarea metodei de interpolare.
- Generarea cadrelor intermediare.
- Vizualizarea si exportul videoclipului rezultat.
- Compararea vizuala a rezultatelor obtinute prin metode diferite.
- Afisarea metricilor de calitate si performanta.

## 6. Tehnologii avute in vedere

- Python
- OpenCV
- PyTorch
- NumPy
- FFmpeg
- Gradio sau o interfata similara

Lista tehnologiilor poate fi ajustata pe parcursul dezvoltarii.
