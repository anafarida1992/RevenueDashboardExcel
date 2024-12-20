**Revenue Dashboard Biscuit Company (Excel)**\
file : https://drive.google.com/drive/folders/14LIFkSGzKBFPX_cop6-ebhz7clVnCqSB?usp=drive_link
\
\
**Insights:**\
\
**A.	Sales Performance**
1. Sales Overview\
• Quantity produk yang terjual sebanyak 3 juta barang, dimana revenue $61.5M dan cost $34.8M sehingga profit yang diperoleh sebesar $26.8M atau 44% margin.
2. Product Overview\
•	Produk dengan kontribusi persentase profit tertinggi adalah shortbread = 41% dengan quantity pembelian 311 ribu, vanilla wafers = 22% dengan quantity pembelian 322 ribu, dan ginger snaps = 17% dengan quantity pembelian 321 ribu.\
•	Produk dengan potensi margin profit per item terbesar adalah shortbread dengan harga jual $45, cost $10, profit $35 atau 78%, vanilla wafers dengan harga jual $36, cost $18, profit $18 atau 50%, ginger snaps dengan harga jual $28, cost $14, profit $14 atau 50%.

**B.	Customer Demography**
1.	Customer Segmentation\
• Kontribusi persentase revenue tertinggi berdasarkan age-group adalah 24.1% berusia 60-74 tahun, dan berdasarkan gender adalah 84% pria.
2.	Geographic Distribution\
• Kontribusi profit tertinggi berdasarkan lokasi customer adalah San Antonio dengan kontribusi persentase revenue 11.9% dari total.
3.	Sales Segmentation\
• Sales person Travis Doyle berkontribusi profit tertinggi yaitu $4.8M atau 18%. Customer Robert Hernandez melakukan pembelian sebanyak 40 ribu barang dengan profit $402k, berkontribusi 1.5% dari total.
4.	Buying Preferences\
• Produk ber-harga lebih dari $10 (expensive) terjual sebanyak 2.1juta, dengan kontribusi persentase revenue 90%. Debit card merupakan metode payment dengan kontribusi persentase revenue tertinggi yaitu 25.4%.

**C.	Revenue Growth Analysis**
1.	Daily\
•	Tertinggi adalah Friday sebesar $9.1M berkontribusi 14.8%.\
•	Terendah adalah Sunday sebesar $8.4M berkontribusi 13.7%.

2.	Monthly\
•	Tertinggi adalah January sebesar $7.9M berkontribusi 12.8%.\
•	Terendah adalah December sebesar $2M berkontribusi 3%.\
•	Growth antara January - December sebesar -$5.9M (-75%).

3.	Quarterly\
•	Tertinggi adalah Q1 (Jan-Mar) sebesar $22.1M berkontribusi 35.9%.\
•	Terendah adalah Q4 (Oct-Dec) sebesar $6.3M berkontribusi 10.3%.\
•	Growth antara Q1-Q4 sebesar -$15.8M (-48%).

**Data Processing:**\
\
**A.	Data Collection**\
• Data yang akan diolah, diperoleh dari sumber data.

**B.	Data Cleaning**\
•	Memastikan data yang akan dianalisis bebas dari data duplikat, nilai kosong, outlier, dan inkonsistensi format.\
•	Mengubah format data agar konsisten. Mengubah format data berupa datetime pada kolom “Transaction Date” dan “Buyer Date of Birth”.\
•	Tidak ada data duplikat, nilai kosong, dan outlier.

**C.	Data Transformation**\
•	Mengubah data mentah menjadi format yang lebih mudah untuk dianalisis.

1.	Feature Engineering\
•	“Age” dihasilkan dari selisih antara “Buyer Date of Birth” dan “Transaction Date”.\
•	“Revenue” dihasilkan dari perkalian “Quantity Purchased” dengan “Unit Price”.\
•	“COGS” (Cost Of Good Sold) dihasilkan dari perkalian “Quantity Purchased” dengan “Cost”.\
•	“Profit” dihasilkan dari selisih “Revenue” dengan “COGS”.\
•	“Full Name” dihasilkan dari penggabungan “Buyer First Name” dan “Buyer Last Name”.\
•	“Weekday” dihasilkan dari nama hari pada “Transaction Date”.\

2.	Labeling\
•	“Age-Group” merupakan pengelompokkan dari “Age” (15-29, 30-44, 45-59, 60-74, 75-89).\
•	“Price Range” merupakan pengelompokkan dari “Unit Price” (jika lebih dari $10 = expensive dan jika kurang dari $10 = cheap).\
•	“Weektype” merupakan pengelompokkan dari “Weekday” (jika Saturday dan Sunday = weekend, maka selain itu = weekday).\

3.	Aggregating\
• Agar mendapatkan insight dari data dengan ringkasan statistik.\
•	“Transaction Date” dikelompokkan menjadi total periode bulanan/monthly dan quarterly.\
