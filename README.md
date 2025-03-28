## #1

두 개의 포트폴리오 $P_1$과 $P_2$의 가중치가 다음과 같이 주어질 때,

$\omega^* = a + b R_{p1}$

$\omega^* = a + b R_{p2}$

이 식은 포트폴리오의 가중치가 상수 $a$와 기대수익률 $R_p$의 선형 결합으로 표현될 수 있음을 의미한다.

임의의 비율 $\lambda$를 사용하여 두 개의 포트폴리오를 조합한 새로운 포트폴리오 $\omega_c$를 정의한다. 

$\omega_c = \lambda \omega^* + (1 - \lambda) \omega^*$

즉, **포트폴리오 $P_1$과 $P_2$를 적절한 비율로 조합하여 새로운 포트폴리오 $C$를 구성할 수 있음**을 보여준다.  

조합된 포트폴리오의 기대수익률 $R_c$는 다음과 같이 정의된다.  

$R_c = \lambda R_{p1} + (1 - \lambda) R_{p2}$

즉, 두 개의 포트폴리오의 기대수익률을 **가중 평균 형태로 표현할 수 있음**을 보여준다.  

이제 조합된 포트폴리오의 가중치를 위 식을 이용해 변형해 봅니다.  

$\omega_c = \lambda (a + b R_{p1}) + (1 - \lambda)(a + b R_{p2})$

$= \lambda a + \lambda b R_{p1} + (1 - \lambda)a + (1 - \lambda)b R_{p2}$

$= a (\lambda + 1 - \lambda) + b (\lambda R_{p1} + (1 - \lambda) R_{p2})$

$= a + b R_c$

이 결과는 조합된 포트폴리오 $\omega_c$도 **원래의 포트폴리오 가중치 표현 $a + bR$과 동일한 형태를 유지함**을 보여준다.  

결론적으로,  
**임의의 포트폴리오도 두 개의 특정한 포트폴리오 $P_1$과 $P_2$의 조합으로 표현될 수 있음**이 증명되었다.  

이는 **Mean-Variance Frontier(평균-분산 경계)** 상의 모든 포트폴리오가 단 두 개의 특정한 포트폴리오를 이용해 표현될 수 있음을 의미하며,  
이를 통해 **Two-Fund Separation Theorem이 성립**함을 보여준다.

---

## #2

#### Consumption-Based CAPM (C-CAPM)의 핵심 공식**  
C-CAPM은 소비와 자산 가격 간의 관계를 설명한다.
자산 $i$의 현재 가격 $P_{i,t}$는 다음과 같이 표현된다:  

$P_{i,t} = E_t \big[ P_{t,t+1} \times {{1}\over{1}}  \big]$

$\frac{U_c(C_{t+1}^*)}{U_c(C_t^*)}$

여기서  
- $P_{t,t+1}$ : 미래 현금 흐름 (수익 포함)  
- $U_c(C)$ : 소비의 한계 효용 (\( U_c > 0, U_{cc} < 0 \))  
- $C_t^*, C_{t+1}^*$ : 최적 소비 수준  

즉, **미래 현금 흐름은 현재 소비와 미래 소비의 한계 효용 비율에 따라 할인된다.**  

#### **시장 경제 상태와 한계 효용의 변화**  
경제 상태(예: 호황 vs. 불황)에 따라 소비 패턴이 변하면 한계 효용도 변한다.  
- **경기 호황**: 소비 증가 → $U_c(C_{t+1})$ 감소 → 할인율 ($\frac{U_c(C_{t+1}^*)}{U_c(C_t^*)}$) 작아짐  
- **경기 침체**: 소비 감소 → $U_c(C_{t+1})$ 증가 → 할인율 커짐  

즉, **경기 침체일수록 미래 현금 흐름이 더 가치 있게 평가되며, 호황일수록 할인율이 커진다.**  

#### **C-CAPM이 미래 현금 흐름과 경제 상태의 상관관계를 예측하는 이유**  
위 식을 공분산 형태로 변형하면,  

$P_{i,t} = E_t[P_{i,t+1}] E_t[m_{t+1}] + Cov_t(m_{t+1}, P_{i,t+1})$

여기서 $m_{t+1} = \frac{U_c(C_{t+1})}{U_c(C_t)}$ 이므로,  
- **한계 효용이 높은 시기**(경기 침체) → **미래 현금 흐름의 가치는 증가**  
- **한계 효용이 낮은 시기**(경기 호황) → **미래 현금 흐름의 가치는 감소**  

즉, **경제 상태(소비 변동)와 미래 현금 흐름 사이의 상관관계가 자산 가격을 결정하는 중요한 요소가 된다.**  

결론적으로, **C-CAPM은 시장 경제 상태(소비 변동)와 미래 현금 흐름의 상관관계를 반영하여 현재 자산 가격을 결정한다.**  
이는 전통적 CAPM이 시장 포트폴리오와 개별 자산 간의 공분산을 강조하는 것과 차별된다.

