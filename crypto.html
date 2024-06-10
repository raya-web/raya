<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Crypto Trading Platform</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            min-height: 100vh;
        }

        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: linear-gradient(90deg, #1a1a1a, #333);
            padding: 1rem 2rem;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .navbar h1 {
            color: #fff;
            margin: 0;
        }

        .navbar .nav-links {
            display: flex;
            gap: 1rem;
        }

        .navbar .nav-links a {
            color: #fff;
            text-decoration: none;
            font-size: 1rem;
            transition: color 0.3s ease;
        }

        .navbar .nav-links a:hover {
            color: #ccc;
        }

        .navbar .profile, .navbar .login-button {
            display: flex;
            align-items: center;
        }

        .navbar .login-button, .navbar .logout-button {
            background-color: #28a745;
            color: #fff;
            border: none;
            padding: 0.5rem 1rem;
            cursor: pointer;
            font-size: 1rem;
            border-radius: 5px;
            transition: background-color 0.3s ease;
        }

        .navbar .login-button:hover, .navbar .logout-button:hover {
            background-color: #218838;
        }

        .navbar .profile {
            display: none;
            color: #fff;
        }

        .modal {
            display: none;
            position: fixed;
            z-index: 1000;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            overflow: auto;
            background-color: rgba(0,0,0,0.5);
            justify-content: center;
            align-items: center;
        }

        .modal-content {
            background-color: #fff;
            padding: 2rem;
            border-radius: 10px;
            width: 300px;
            text-align: center;
        }

        .modal-content input {
            width: calc(100% - 1rem);
            padding: 0.5rem;
            margin: 0.5rem 0;
            border: 1px solid #ccc;
            border-radius: 5px;
        }

        .modal-content button {
            background-color: #28a745;
            color: #fff;
            border: none;
            padding: 0.5rem 1rem;
            cursor: pointer;
            font-size: 1rem;
            border-radius: 5px;
            transition: background-color 0.3s ease;
        }

        .modal-content button:hover {
            background-color: #218838;
        }

        header {
            background-color: #333;
            color: #fff;
            padding: 1rem;
            text-align: center;
        }

        main {
            flex: 1;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 2rem;
        }

        .chart-container {
            width: 80%;
            max-width: 600px;
            height: 400px;
        }

        .trade-buttons, .transaction-buttons {
            margin-top: 2rem;
        }

        .trade-buttons button, .transaction-buttons button {
            background-color: #28a745;
            color: #fff;
            border: none;
            padding: 1rem 2rem;
            margin: 0 1rem;
            cursor: pointer;
            font-size: 1rem;
            border-radius: 5px;
            transition: background-color 0.3s ease;
        }

        .trade-buttons button:hover, .transaction-buttons button:hover {
            background-color: #218838;
        }

        .trade-buttons button:nth-child(2), .transaction-buttons button:nth-child(2) {
            background-color: #dc3545;
        }

        .trade-buttons button:nth-child(2):hover, .transaction-buttons button:nth-child(2):hover {
            background-color: #c82333;
        }

        footer {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 1rem;
        }

        .transaction-form {
            margin-top: 2rem;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .transaction-form input {
            padding: 0.5rem;
            font-size: 1rem;
            margin-bottom: 1rem;
            border: 1px solid #ccc;
            border-radius: 5px;
        }

        .balance, .profit-loss, .crypto-price {
            margin-top: 2rem;
            font-size: 1.5rem;
        }

        .leverage-input, .amount-input {
            margin-top: 1rem;
            font-size: 1rem;
        }

        .leverage-input label, .amount-input label {
            margin-right: 0.5rem;
        }
    </style>
</head>
<body>
    <div class="navbar">
        <h1>Crypto Trading Platform</h1>
        <div class="nav-links">
            <a href="#">Home</a>
            <a href="#">Markets</a>
            <a href="#">Portfolio</a>
            <a href="#">Contact</a>
        </div>
        <div class="profile" id="userProfile">
            <span id="usernameDisplay"></span>
            <button class="logout-button" onclick="logout()">Logout</button>
        </div>
        <div class="login-button-container">
            <button class="login-button" onclick="showLoginForm()">Login</button>
        </div>
    </div>

    <div id="loginModal" class="modal">
        <div class="modal-content">
            <h2>Login</h2>
            <input type="text" id="loginUsername" placeholder="Username">
            <input type="password" id="loginPassword" placeholder="Password">
            <button onclick="login()">Login</button>
            <button onclick="showRegisterForm()">Register</button>
            <div id="loginError" style="color: red; display: none;">Invalid username or password</div>
        </div>
    </div>

    <div id="registerModal" class="modal">
        <div class="modal-content">
            <h2>Register</h2>
            <input type="text" id="registerUsername" placeholder="Username">
            <input type="password" id="registerPassword" placeholder="Password">
            <button onclick="register()">Register</button>
            <div id="registerError" style="color: red; display: none;">User already exists</div>
        </div>
    </div>

    <main>
        <div class="chart-container">
            <div id="chart" style="width: 100%; height: 400px;"></div>
        </div>
        <div class="balance" id="balanceDisplay">Balance: $100.00</div>
        <div class="profit-loss" id="profitLossDisplay">Profit/Loss: $0.00</div>
        <div class="crypto-price" id="cryptoPriceDisplay">Current Bitcoin Price: $0.00</div>
        <div class="leverage-input">
            <label for="leverage">Leverage:</label>
            <input type="number" id="leverage" value="1" min="1" step="1">
        </div>
        <div class="amount-input">
            <label for="tradingAmount">Amount:</label>
            <input type="number" id="tradingAmount" value="10" min="1" step="1">
        </div>
        <div class="trade-buttons">
            <button onclick="openLong()">Open Long</button>
            <button onclick="closeAllLongs()">Close All Longs</button>
            <button onclick="openShort()">Open Short</button>
            <button onclick="closeAllShorts()">Close All Shorts</button>
        </div>
        <div class="transaction-buttons">
            <button onclick="showDepositForm()">Deposit</button>
            <button onclick="showWithdrawForm()">Withdraw</button>
        </div>
        <div class="transaction-form" id="transactionForm" style="display:none;">
            <input type="number" id="amount" placeholder="Enter amount" min="0.01" step="0.01">
            <button id="transactionButton" onclick="processTransaction()">Submit</button>
        </div>
    </main>
    <footer>
        <p>&copy; 2024 Crypto Trading Platform</p>
    </footer>
   <script src="https://unpkg.com/lightweight-charts/dist/lightweight-charts.standalone.production.js"></script>

    <script>
        const chart = LightweightCharts.createChart(document.getElementById('chart'), {
            width: 600,
            height: 400,
            layout: {
                backgroundColor: '#ffffff',
                textColor: '#000000'
            },
            grid: {
                vertLines: {
                    color: '#e0e0e0'
                },
                horzLines: {
                    color: '#e0e0e0'
                }
            },
            priceScale: {
                borderColor: '#cccccc'
            },
            timeScale: {
                borderColor: '#cccccc'
            }
        });

        const candleSeries = chart.addCandlestickSeries({
            upColor: '#4caf50',
            borderUpColor: '#4caf50',
            wickUpColor: '#4caf50',
            downColor: '#f44336',
            borderDownColor: '#f44336',
            wickDownColor: '#f44336'
        });

        let balance = 100.00;
        let profitLoss = 0.00;
        let bitcoinPrice = 0.00;
        let positions = [];

        async function fetchBitcoinData() {
            try {
                const response = await fetch('https://api.binance.com/api/v3/klines?symbol=BTCUSDT&interval=1m&limit=100');
                const data = await response.json();
                const formattedData = data.map(item => ({
                    time: item[0] / 1000,
                    open: parseFloat(item[1]),
                    high: parseFloat(item[2]),
                    low: parseFloat(item[3]),
                    close: parseFloat(item[4])
                }));
                bitcoinPrice = formattedData[formattedData.length - 1].close;
                candleSeries.setData(formattedData);
                updateDisplay();
            } catch (error) {
                console.error('Error fetching Bitcoin data:', error);
            }
        }

        function updateDisplay() {
            document.getElementById('balanceDisplay').innerText = `Balance: $${balance.toFixed(2)}`;
            document.getElementById('profitLossDisplay').innerText = `Profit/Loss: $${profitLoss.toFixed(2)}`;
            document.getElementById('cryptoPriceDisplay').innerText = `Current Bitcoin Price: $${bitcoinPrice.toFixed(2)}`;
        }

        function openLong() {
            const leverage = parseInt(document.getElementById('leverage').value);
            const amount = parseFloat(document.getElementById('tradingAmount').value);
            const position = { type: 'long', leverage, amount, price: bitcoinPrice };
            positions.push(position);
            alert('Opened Long Position');
        }

        function closeAllLongs() {
            const closedPositions = positions.filter(position => position.type === 'long');
            let pl = 0;
            closedPositions.forEach(position => {
                const priceChange = bitcoinPrice - position.price;
                const profit = priceChange * position.amount * position.leverage;
                pl += profit;
            });
            positions = positions.filter(position => position.type !== 'long');
            profitLoss += pl;
            balance += pl;
            alert('Closed All Long Positions');
            updateDisplay();
        }

        function openShort() {
            const leverage = parseInt(document.getElementById('leverage').value);
            const amount = parseFloat(document.getElementById('tradingAmount').value);
            const position = { type: 'short', leverage, amount, price: bitcoinPrice };
            positions.push(position);
            alert('Opened Short Position');
        }

        function closeAllShorts() {
            const closedPositions = positions.filter(position => position.type === 'short');
            let pl = 0;
            closedPositions.forEach(position => {
                const priceChange = position.price - bitcoinPrice;
                const profit = priceChange * position.amount * position.leverage;
                pl += profit;
            });
            positions = positions.filter(position => position.type !== 'short');
            profitLoss += pl;
            balance += pl;
            alert('Closed All Short Positions');
            updateDisplay();
        }

        function showDepositForm() {
            const transactionForm = document.getElementById('transactionForm');
            const transactionButton = document.getElementById('transactionButton');
            transactionForm.style.display = 'block';
            transactionButton.innerText = 'Deposit';
            transactionButton.onclick = () => processTransaction('deposit');
        }

        function showWithdrawForm() {
            const transactionForm = document.getElementById('transactionForm');
            const transactionButton = document.getElementById('transactionButton');
            transactionForm.style.display = 'block';
            transactionButton.innerText = 'Withdraw';
            transactionButton.onclick = () => processTransaction('withdraw');
        }

        function processTransaction(type) {
            const amount = parseFloat(document.getElementById('amount').value);
            if (type === 'deposit') {
                balance += amount;
                alert(`Deposited $${amount.toFixed(2)}`);
            } else if (type === 'withdraw') {
                if (amount <= balance) {
                    balance -= amount;
                    alert(`Withdrew $${amount.toFixed(2)}`);
                } else {
                    alert('Insufficient balance');
                }
            }
            document.getElementById('transactionForm').style.display = 'none';
            updateDisplay();
        }

        function showLoginForm() {
            document.getElementById('loginModal').style.display = 'flex';
            document.getElementById('registerModal').style.display = 'none';
        }

        function showRegisterForm() {
            document.getElementById('registerModal').style.display = 'flex';
            document.getElementById('loginModal').style.display = 'none';
        }

        function login() {
            const username = document.getElementById('loginUsername').value;
            const password = document.getElementById('loginPassword').value;
            const storedUser = JSON.parse(localStorage.getItem(username));

            if (storedUser && storedUser.password === password) {
                localStorage.setItem('loggedInUser', username);
                document.getElementById('usernameDisplay').innerText = `Welcome, ${username}`;
                document.querySelector('.profile').style.display = 'flex';
                document.querySelector('.login-button-container').style.display = 'none';
                document.getElementById('loginModal').style.display = 'none';
                document.getElementById('loginError').style.display = 'none';
                alert('Logged in as ' + username);
            } else {
                document.getElementById('loginError').style.display = 'block';
            }
        }

        function logout() {
            localStorage.removeItem('loggedInUser');
            document.getElementById('usernameDisplay').innerText = '';
            document.querySelector('.profile').style.display = 'none';
            document.querySelector('.login-button-container').style.display = 'flex';
            alert('Logged out');
        }

        function register() {
            const username = document.getElementById('registerUsername').value;
            const password = document.getElementById('registerPassword').value;
            const storedUser = JSON.parse(localStorage.getItem(username));

            if (!storedUser) {
                localStorage.setItem(username, JSON.stringify({ password: password }));
                localStorage.setItem('loggedInUser', username);
                document.getElementById('usernameDisplay').innerText = `Welcome, ${username}`;
                document.querySelector('.profile').style.display = 'flex';
                document.querySelector('.login-button-container').style.display = 'none';
                document.getElementById('registerModal').style.display = 'none';
                document.getElementById('registerError').style.display = 'none';
                alert('Registered and logged in as ' + username);
            } else {
                document.getElementById('registerError').style.display = 'block';
            }
        }

        window.onload = function() {
            const loggedInUser = localStorage.getItem('loggedInUser');
            if (loggedInUser) {
                document.getElementById('usernameDisplay').innerText = `Welcome, ${loggedInUser}`;
                document.querySelector('.profile').style.display = 'flex';
                document.querySelector('.login-button-container').style.display = 'none';
            }
            fetchBitcoinData();
            setInterval(fetchBitcoinData, 60000); // Refresh data every minute
        };
    </script>
</body>
</html>
