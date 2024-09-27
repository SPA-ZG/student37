URL moje aplikacije je: https://web-project6.vercel.app/

1.interpolation/one-way binding - u src/components/BlogPost.vue na 5oj i 6oj liniji ispisuju se title i content kao primjer one way bindinga.
2.two-way binding - u src/components/CommentSection.vue od 13 do 15 linije moze se vidjeti primjer two way bindinga gdje kad upisujemo komentar u isto vrijeme se mijenja 
							polje u kojem se prikazuje "Pregled komentara". To se moze vidjeti i u aplikaciji kad se otvori neki blog i proba upisati komentar.
3.methods - metode su koristene i u BlogPost.vue i CommentSection.vue spomenutim komponentama
4.computed properties - u src/components/BlogList.vue na 24oj liniji moze se vidjeti koristenje computed propertiesa. Dakle provjerava se je li 
								content(sadrzaj) bloga dulji od 100 znakova te ako jeste prikazuje se samo prvih 100 i dodaju tri tocke, a ako nije 
                        prikaze se cijeli sadrzaj.
5.barem jedan scoped style - scoped styleovi su koristeni u svim komponentama
6.koristiti barem jedan lifecycle hook - koristen je u src/components/BlogPost.vue na 31oj liniji koda
7.routing (više stranica) - implementirano je i to moze se provjeriti src/router.js folderu i za linkove i za "catch all"
	aplikacija mora biti bookmarkable, tako da rade linkovi (ne samo na root, već i moj-web.com/stranica1, moj-web.com/stranica2)
	dinamičko usmjeravanje s 404 stranicom ("catch all")
8.(barem) dvije komponente
	komponenta bez stanja, koristiti properties - src/components/BlogList.vue
	komponenta sa stanjem - src/components/BlogPost.vue
9.barem jedna komponenta mora emitirati barem jedan event - src/components/CommentSection.vue 60. linija koda imamo emit te se onda u 
				src/components/BlogPost.vue osluškuje događanja preko 'comment-added'(9. linija koda)
   				te se ažurira broj komentara
10.store (Pinia) - src/store/blogStore.js
						Korišteno za dohvat broja blogova u src/views/HomePage.vue (29. linija koda)
11.asinkroni dohvat podataka s backenda:
	Korišten je firebase. U src/components/BlogPost.vue mozemo vidjeti od 37. do 49. linije koda korištenje asinkronog dohvata.




