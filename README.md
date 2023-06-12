# JPMC Task 3
Starter repo for task 3 of JPMC's Forage program

python -m venv myenv
myenv\Scripts\activate
pip install -r datafeed/requirements.txt
npm install

python datafeed/server3.py
npm start

netstat -ano | findstr :3000
for /f "tokens=5" %a in ('netstat -ano ^| findstr :3000') do taskkill /f /pid %a