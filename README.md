location.href = 'https://uigradients.com';
e = document.querySelectorAll('.palette__gradient');
x = "";
for(i = 0; i < e.length; i++){
	x += "."+e[i].firstChild.innerHTML.replace(' ', '-')+"{background: "+e[i].style.background+";}";
}