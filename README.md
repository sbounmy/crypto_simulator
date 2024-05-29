# crypto_simulator
Bitcoin and Ethereum Simulator for "If I had bought ..."

```
simulator = Simulator::Bitcoin.new(since: 5.years.ago, every: :month, amount: 100, fiat: :eur)

simulator.btc.total # 76.03 BTC
simulator.btc.buy_price 
simulator.btc_price_average # 4_940_000 €
simulator.fiat.total # 6_000 €
simulator.fiat.now # 4_940_000 €
simulator.roi.percent # 99%
simulator.roi.fiat # 4_939_000 €

# todo for charts
simulator.points # for charts
```

Params :
- since: Date to calculate from
- every: :day, :week, :month, :year
- amount: decimal
- fiat: :eur or :dollar
