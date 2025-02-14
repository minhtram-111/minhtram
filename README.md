noBtn.addEventListener("mouseover"), () => {
  const newX = Math.floor(Math.random() *
                          questionContainer.offsetWidth);
  const newY = Math.floor(Math.random() *
                          questionContainer.offsetWidth);
  
  noBtn.style.left = '${newX}px';
  noBtn.style.top = '${newY}px';
});

yesBtn.assEventListener("click", () => {
  const timeoutId = setTimeout(() => {
    heartLoader.style.display = "none";
    resultContainer.style.display = "inheit"; 
    gifResult.play();
    }, 3000);
});
