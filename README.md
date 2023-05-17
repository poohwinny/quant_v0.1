# yun_quant_v0.1

!pip install bokeh
!pip install -q finance-datareader

import FinanceDataReader as fdr

# KRX stock delisting symbol list 상장폐지 종목 전체 리스트
krx_delisting = fdr.StockListing('KRX-DELISTING')
krx_delisting

# 상장폐지 종목 일자별 데이터
df = fdr.DataReader('056000', exchange='KRX-DELISTING')
df
