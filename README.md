# Project Test Backend CRUD Export Import

## Step 1
Membuat Database Bernama "test_backend"

## Step 2
.env yang berisikan:
```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=test_backend
DB_USERNAME=root
DB_PASSWORD=
```

## Step 3
php artisan migrate

## Step 4
php artisan serve

## Step 5
Link API:

Get Karyawan: <br>
* localhost:8000/api/karyawan?limit=5&page=1 


Create Karyawan:
[a relative link](localhost:8000/api/karyawan)
Body Create: 
```json
{
"nama":"",
"nomor":"",
"jabatan":"",
"departement":"",
"tanggal_masuk":"",
"status": "",
 "foto": ""
}
```


Update Karyawan:
localhost:8000/api/karyawan/{id}
Body Update: {
    "nama":"",
	"nomor":"",
	"jabatan":"",
	"departement":"",
	"tanggal_masuk":"",
    "status": "",
    "foto": ""
}

Delete Karyawan: 
localhost:8000/api/karyawan/{id}


Import Karyawan: 
localhost:8000/api/karyawan/import
Body: {
    "file" : "",
}

Export Csv Karyawan: 
localhost:8000/api/karyawan/export-csv

Export PDF Karyawan: 
localhost:8000/api/karyawan/export-pdf
