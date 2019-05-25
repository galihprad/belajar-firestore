# belajar-firestore


#### Get Data

```JavaScript
db.collection('cafe').get().then((snapshot)=>{
	snapshot.docs.forEach(doc=>{
		console.log(doc.data());
	});
})

```


#### Add Data
```javaScript
form.addEventListener('submit',(e)=>{
	e.preventDefault();
	db.collection('cafe').add({
		nama:form.nama.value,
		lokasi:form.lokasi.value

	})
	form.nama.value='';
	form.lokasi.value='';
})
```
