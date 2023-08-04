# Verilog-layer1-MPtest

![image](https://github.com/YunJoongChul/Verilog-layer1-MPtest/assets/86291432/b2075d5f-f446-49d9-bdd9-1ffd954e4088)


1.test 결과 2clk 밀림 따라서 cnt_module 에서 2보다작을때 까지 cnt_ctrl 0 걸고 그 후에 증가시킴

![image](https://github.com/YunJoongChul/Verilog-layer1-MPtest/assets/86291432/99f4de84-a8a0-4448-9479-69ff31ae252b)

2. cnt_ctrl 1일시 high 2일시 low
3. high 비교 reg때문 1clk 밀리고 low 비교 reg 떄문에 1clk 밀림 그래서 결과 max값 출력하는데 총 4clk delay 생김
4. 따라서 주소값을 cnt_module < 5 보다 작을때까지 0으로 시키고 그 이후에 증가 시키도록함.
5. wea신호는 이제 마스터 한듯 주소값 올리기 직전에 켜주면 됨.
