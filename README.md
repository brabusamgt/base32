# base32
Real-Time Base Mempool Monitoring Python Example:
from web3 import Web3

w3 = Web3(Web3.WebsocketProvider("wss://mainnet.base.org"))

def handle(tx):
    print("New tx:", tx)

w3.eth.subscribe("pendingTransactions", handle)
Great for bots and analytics.
