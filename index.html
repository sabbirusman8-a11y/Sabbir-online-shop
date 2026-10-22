
<!DOCTYPE html>
<html lang="bn">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Sabbir Online Shop</title>
<style>
body{font-family:Arial,sans-serif;background:#f2f6f4;padding:15px}
header{background:#087f5b;color:white;padding:18px;border-radius:12px}
section{background:white;padding:16px;margin-top:15px;border-radius:12px}
input,button{box-sizing:border-box;width:100%;padding:12px;margin:7px 0}
button{background:#087f5b;color:white;border:0;border-radius:8px}
.product{border:1px solid #ddd;border-radius:10px;padding:10px;margin-top:12px}
.product img{width:100%;max-height:220px;object-fit:contain}
</style>
</head>
<body>
<header>
<h2>Sabbir Online Shop</h2>
<p>আপনার অনলাইন দোকান</p>
</header>

<section>
<h3>নতুন পণ্য যোগ করুন</h3>
<label>পণ্যের ছবি নির্বাচন করুন</label>
<input id="photo" type="file" accept="image/*">
<img id="preview" style="display:none;width:100%;max-height:200px;object-fit:contain">
<input id="name" placeholder="পণ্যের নাম">
<input id="price" type="number" placeholder="পণ্যের দাম (টাকা)">
<button onclick="addProduct()">পণ্য যোগ করুন</button>
</section>

<section>
<h3>আমাদের পণ্য</h3>
<div id="products"></div>
</section>

<script>
let products=[];
try {
 products=JSON.parse(localStorage.getItem("sabbirProducts")||"[]");
} catch(e) { products=[]; }

const photo=document.getElementById("photo");
photo.addEventListener("change",function(){
 const file=this.files[0];
 if(!file)return;
 if(file.size>1500000){
  alert("দয়া করে ১.৫ MB-এর চেয়ে ছোট ছবি বেছে নিন।");
  this.value="";
  return;
 }
 const reader=new FileReader();
 reader.onload=function(){
  const preview=document.getElementById("preview");
  preview.src=reader.result;
  preview.style.display="block";
 };
 reader.readAsDataURL(file);
});

function showProducts(){
 const box=document.getElementById("products");
 box.innerHTML="";
 if(!products.length){
  box.textContent="এখনো কোনো পণ্য যোগ করা হয়নি।";
  return;
 }
 products.forEach(p=>{
  const div=document.createElement("div");
  div.className="product";
  if(p.photo){
   const img=document.createElement("img");
   img.src=p.photo;
   img.alt=p.name;
   div.appendChild(img);
  }
  const title=document.createElement("h3");
  title.textContent=p.name;
  const price=document.createElement("p");
  price.textContent="দাম: ৳"+p.price;
  div.appendChild(title);
  div.appendChild(price);
  box.appendChild(div);
 });
}

function addProduct(){
 const name=document.getElementById("name").value.trim();
 const price=document.getElementById("price").value;
 const preview=document.getElementById("preview");
 if(!name||price===""||Number(price)<0){
  alert("পণ্যের নাম ও সঠিক দাম লিখুন।");
  return;
 }
 products.push({
  name:name,
  price:price,
  photo:preview.style.display==="none"?"":preview.src
 });
 try{
  localStorage.setItem("sabbirProducts",JSON.stringify(products));
 }catch(e){
  products.pop();
  alert("ছবি সংরক্ষণ করা যায়নি। ছোট ছবি দিয়ে আবার চেষ্টা করুন।");
  return;
 }
 document.getElementById("name").value="";
 document.getElementById("price").value="";
 photo.value="";
 preview.src="";
 preview.style.display="none";
 showProducts();
 alert("পণ্য যোগ হয়েছে!");
}
showProducts();
</script>
</body>
</html>
