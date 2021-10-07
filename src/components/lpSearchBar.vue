<template>
    <div class="search">
        <!-- The search bar -->
        <input autofocus id="searchbar" placeholder="Type your data. . ." autocomplete="off">
        <button type="button" id="btnS" class="btn-search"><i class="fas fa-search"></i></button>
    </div>
</template>


<style scoped>

button:hover { text-shadow: 0 5px 10px rgba(255,255,255,0.2); }

button a i { color: #ddd; }
button:hover a i { color: white; }

button
{
	background-color: transparent;
	border: none;
	margin: 12px;
	transition: 0.15s;
	font-size: 14px;
	display: none;
}

button:hover
{
	transform: translateY(-3px);
	cursor: pointer;
}

button a i { font-size: 32px !IMPORTANT; }


.search {
	width: 450px;
	border: none;
	border-radius: 5px;
	transition: 0.15s;
	display: flex;
  justify-content: space-between;
  background-color: rgba(255, 255, 255, 0.938); 
	border-bottom: 4px solid #7fd4ff;
  
}

.search:hover
{
	background-color: #eee;
	box-shadow: 0 0 10px rgba(0,0,0,0.3);
	border-bottom: 4px solid #C1B3FF;
}

.search:focus { background-color: #fff; }


/* The searchbar */
#searchbar
{
	width: 450px;
	background-color: transparent;
	border: none;
	border-radius: 5px;
	padding: 12px 20px;
}

.btn-search {
	color: #a5a5a5;
}

input {
  outline: none;
}

</style>