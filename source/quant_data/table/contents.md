# 1_ods_jqdata

## concept_all 获取概念列表

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | date | date |  |  | √ |  |  |  | 日期 | 
 | 2 | code | varchar | 50 |  | √ |  |  |  | 概念代码 | 
 | 3 | name | varchar | 50 |  |  |  | √ |  | 概念名称 | 
 | 4 | start_date | date |  |  |  |  | √ |  | 开始日期 | 

## concept_stocks 获取概念成分股

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | date | date |  |  | √ |  |  |  | 日期 | 
 | 2 | concept_code | varchar | 50 |  | √ |  |  |  | 概念代码 | 
 | 3 | stock_code | varchar | 50 |  | √ |  |  |  | 股票代码 | 

## index_all 获取 A 股市场指数及其简要概况

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | code | varchar | 50 |  | √ |  |  |  | 指数代码 | 
 | 2 | display_name | varchar | 50 |  |  |  | √ |  | 中文名称 | 
 | 3 | name | varchar | 50 |  |  |  | √ |  | 简称 | 
 | 4 | start_date | date |  |  |  |  | √ |  | 上市日期 | 
 | 5 | end_date | date |  |  |  |  | √ |  | 退市日期，如果没有退市则为2200-01-01 | 
 | 6 | type | varchar | 50 |  |  |  | √ |  | 类型 | 

## index_daily_price 指数每日行情

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | date | date |  |  | √ |  |  |  | 日期 | 
 | 2 | code | varchar | 50 |  | √ |  |  |  | 指数代码 | 
 | 3 | open | float | 12 |  |  |  | √ |  | 开盘价 | 
 | 4 | close | float | 12 |  |  |  | √ |  | 收盘价 | 
 | 5 | low | float | 12 |  |  |  | √ |  | 最低价 | 
 | 6 | high | float | 12 |  |  |  | √ |  | 最高价 | 
 | 7 | volume | float | 12 |  |  |  | √ |  | 成交量 | 
 | 8 | money | float | 12 |  |  |  | √ |  | 成交额 | 
 | 9 | vwap | float | 12 |  |  |  | √ |  | 成交量加权均价 | 
 | 10 | pre_close | float | 12 |  |  |  | √ |  | 昨日收盘价 | 

## industry_all_sw_l1 获取申万一级行业列表

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | date | date |  |  | √ |  |  |  | 日期 | 
 | 2 | code | varchar | 50 |  | √ |  |  |  | 行业代码 | 
 | 3 | name | varchar | 50 |  |  |  | √ |  | 行业名称 | 
 | 4 | start_date | date |  |  |  |  | √ |  | 开始日期 | 

## industry_all_sw_l2 获取申万二级行业列表

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | date | date |  |  | √ |  |  |  | 日期 | 
 | 2 | code | varchar | 50 |  | √ |  |  |  | 行业代码 | 
 | 3 | name | varchar | 50 |  |  |  | √ |  | 行业名称 | 
 | 4 | start_date | date |  |  |  |  | √ |  | 开始日期 | 

## industry_all_sw_l3 获取申万三级行业列表

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | date | date |  |  | √ |  |  |  | 日期 | 
 | 2 | code | varchar | 50 |  | √ |  |  |  | 行业代码 | 
 | 3 | name | varchar | 50 |  |  |  | √ |  | 行业名称 | 
 | 4 | start_date | date |  |  |  |  | √ |  | 开始日期 | 

## industry_stocks_sw_l1 获取申万一级行业成分股

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | date | date |  |  | √ |  |  |  | 日期 | 
 | 2 | industry_code | varchar | 50 |  | √ |  |  |  | 行业代码 | 
 | 3 | stock_code | varchar | 50 |  | √ |  |  |  | 股票代码 | 

## industry_stocks_sw_l2 获取申万二级行业成分股

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | date | date |  |  | √ |  |  |  | 日期 | 
 | 2 | industry_code | varchar | 50 |  | √ |  |  |  | 行业代码 | 
 | 3 | stock_code | varchar | 50 |  | √ |  |  |  | 股票代码 | 

## industry_stocks_sw_l3 获取申万三级行业成分股

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | date | date |  |  | √ |  |  |  | 日期 | 
 | 2 | industry_code | varchar | 50 |  | √ |  |  |  | 行业代码 | 
 | 3 | stock_code | varchar | 50 |  | √ |  |  |  | 股票代码 | 

## stock_all 获取 A 股市场全体股票及其简要概况

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | code | varchar | 50 |  | √ |  |  |  | 股票代码 | 
 | 2 | display_name | varchar | 50 |  |  |  | √ |  | 中文名称 | 
 | 3 | name | varchar | 50 |  |  |  | √ |  | 简称 | 
 | 4 | start_date | date |  |  |  |  | √ |  | 上市日期 | 
 | 5 | end_date | date |  |  |  |  | √ |  | 退市日期，如果没有退市则为2200-01-01 | 
 | 6 | type | varchar | 50 |  |  |  | √ |  | 类型 | 

## stock_daily_balance 股票季度资产负债表

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | date | date |  |  | √ |  |  |  | 日期 | 
 | 2 | code | varchar | 50 |  | √ |  |  |  | 股票代码 | 
 | 3 | pubDate | date |  |  |  |  | √ |  | 公司发布财报日期 | 
 | 4 | statDate | date |  |  |  |  | √ |  | 财报统计的季度的最后一天 | 
 | 5 | cash_equivalents | float | 12 |  |  |  | √ |  | 货币资金(元) | 
 | 6 | settlement_provi | float | 12 |  |  |  | √ |  | 结算备付金(元) | 
 | 7 | lend_capital | float | 12 |  |  |  | √ |  | 拆出资金(元) | 
 | 8 | trading_assets | float | 12 |  |  |  | √ |  | 交易性金融资产(元) | 
 | 9 | bill_receivable | float | 12 |  |  |  | √ |  | 应收票据(元) | 
 | 10 | account_receivable | float | 12 |  |  |  | √ |  | 应收账款(元) | 
 | 11 | advance_payment | float | 12 |  |  |  | √ |  | 预付款项(元) | 
 | 12 | insurance_receivables | float | 12 |  |  |  | √ |  | 应收保费(元) | 
 | 13 | reinsurance_receivables | float | 12 |  |  |  | √ |  | 应收分保账款(元) | 
 | 14 | reinsurance_contract_reserves_receivable | float | 12 |  |  |  | √ |  | 应收分保合同准备金(元) | 
 | 15 | interest_receivable | float | 12 |  |  |  | √ |  | 应收利息(元) | 
 | 16 | dividend_receivable | float | 12 |  |  |  | √ |  | 应收股利(元) | 
 | 17 | other_receivable | float | 12 |  |  |  | √ |  | 其他应收款(元) | 
 | 18 | bought_sellback_assets | float | 12 |  |  |  | √ |  | 买入返售金融资产(元) | 
 | 19 | inventories | float | 12 |  |  |  | √ |  | 存货(元) | 
 | 20 | non_current_asset_in_one_year | float | 12 |  |  |  | √ |  | 一年内到期的非流动资产(元) | 
 | 21 | other_current_assets | float | 12 |  |  |  | √ |  | 其他流动资产(元) | 
 | 22 | total_current_assets | float | 12 |  |  |  | √ |  | 流动资产合计(元) | 
 | 23 | loan_and_advance | float | 12 |  |  |  | √ |  | 发放委托贷款及垫款(元) | 
 | 24 | hold_for_sale_assets | float | 12 |  |  |  | √ |  | 可供出售金融资产(元) | 
 | 25 | hold_to_maturity_investments | float | 12 |  |  |  | √ |  | 持有至到期投资(元) | 
 | 26 | longterm_receivable_account | float | 12 |  |  |  | √ |  | 长期应收款(元) | 
 | 27 | longterm_equity_invest | float | 12 |  |  |  | √ |  | 长期股权投资(元) | 
 | 28 | investment_property | float | 12 |  |  |  | √ |  | 投资性房地产(元) | 
 | 29 | fixed_assets | float | 12 |  |  |  | √ |  | 固定资产(元) | 
 | 30 | constru_in_process | float | 12 |  |  |  | √ |  | 在建工程(元) | 
 | 31 | construction_materials | float | 12 |  |  |  | √ |  | 工程物资(元) | 
 | 32 | fixed_assets_liquidation | float | 12 |  |  |  | √ |  | 固定资产清理(元) | 
 | 33 | biological_assets | float | 12 |  |  |  | √ |  | 生产性生物资产(元) | 
 | 34 | oil_gas_assets | float | 12 |  |  |  | √ |  | 油气资产(元) | 
 | 35 | intangible_assets | float | 12 |  |  |  | √ |  | 无形资产(元) | 
 | 36 | development_expenditure | float | 12 |  |  |  | √ |  | 开发支出(元) | 
 | 37 | good_will | float | 12 |  |  |  | √ |  | 商誉(元) | 
 | 38 | long_deferred_expense | float | 12 |  |  |  | √ |  | 长期待摊费用(元) | 
 | 39 | deferred_tax_assets | float | 12 |  |  |  | √ |  | 递延所得税资产(元) | 
 | 40 | other_non_current_assets | float | 12 |  |  |  | √ |  | 其他非流动资产(元) | 
 | 41 | total_non_current_assets | float | 12 |  |  |  | √ |  | 非流动资产合计(元) | 
 | 42 | total_assets | float | 12 |  |  |  | √ |  | 资产总计(元) | 
 | 43 | shortterm_loan | float | 12 |  |  |  | √ |  | 短期借款(元) | 
 | 44 | borrowing_from_centralbank | float | 12 |  |  |  | √ |  | 向中央银行借款(元) | 
 | 45 | deposit_in_interbank | float | 12 |  |  |  | √ |  | 吸收存款及同业存放(元) | 
 | 46 | borrowing_capital | float | 12 |  |  |  | √ |  | 拆入资金(元) | 
 | 47 | trading_liability | float | 12 |  |  |  | √ |  | 交易性金融负债(元) | 
 | 48 | notes_payable | float | 12 |  |  |  | √ |  | 应付票据(元) | 
 | 49 | accounts_payable | float | 12 |  |  |  | √ |  | 应付账款(元) | 
 | 50 | advance_peceipts | float | 12 |  |  |  | √ |  | 预收款项(元) | 
 | 51 | sold_buyback_secu_proceeds | float | 12 |  |  |  | √ |  | 卖出回购金融资产款(元) | 
 | 52 | commission_payable | float | 12 |  |  |  | √ |  | 应付手续费及佣金(元) | 
 | 53 | salaries_payable | float | 12 |  |  |  | √ |  | 应付职工薪酬(元) | 
 | 54 | taxs_payable | float | 12 |  |  |  | √ |  | 应交税费(元) | 
 | 55 | interest_payable | float | 12 |  |  |  | √ |  | 应付利息(元) | 
 | 56 | dividend_payable | float | 12 |  |  |  | √ |  | 应付股利(元) | 
 | 57 | other_payable | float | 12 |  |  |  | √ |  | 其他应付款(元) | 
 | 58 | reinsurance_payables | float | 12 |  |  |  | √ |  | 应付分保账款(元) | 
 | 59 | insurance_contract_reserves | float | 12 |  |  |  | √ |  | 保险合同准备金(元) | 
 | 60 | proxy_secu_proceeds | float | 12 |  |  |  | √ |  | 代理买卖证券款(元) | 
 | 61 | receivings_from_vicariously_sold_securities | float | 12 |  |  |  | √ |  | 代理承销证券款(元) | 
 | 62 | non_current_liability_in_one_year | float | 12 |  |  |  | √ |  | 一年内到期的非流动负债(元) | 
 | 63 | other_current_liability | float | 12 |  |  |  | √ |  | 其他流动负债(元) | 
 | 64 | total_current_liability | float | 12 |  |  |  | √ |  | 流动负债合计(元) | 
 | 65 | longterm_loan | float | 12 |  |  |  | √ |  | 长期借款(元) | 
 | 66 | bonds_payable | float | 12 |  |  |  | √ |  | 应付债券(元) | 
 | 67 | longterm_account_payable | float | 12 |  |  |  | √ |  | 长期应付款(元) | 
 | 68 | specific_account_payable | float | 12 |  |  |  | √ |  | 专项应付款(元) | 
 | 69 | estimate_liability | float | 12 |  |  |  | √ |  | 预计负债(元) | 
 | 70 | deferred_tax_liability | float | 12 |  |  |  | √ |  | 递延所得税负债(元) | 
 | 71 | other_non_current_liability | float | 12 |  |  |  | √ |  | 其他非流动负债(元) | 
 | 72 | total_non_current_liability | float | 12 |  |  |  | √ |  | 非流动负债合计(元) | 
 | 73 | total_liability | float | 12 |  |  |  | √ |  | 负债合计(元) | 
 | 74 | paidin_capital | float | 12 |  |  |  | √ |  | 实收资本(或股本)(元) | 
 | 75 | capital_reserve_fund | float | 12 |  |  |  | √ |  | 资本公积金(元) | 
 | 76 | treasury_stock | float | 12 |  |  |  | √ |  | 库存股(元) | 
 | 77 | specific_reserves | float | 12 |  |  |  | √ |  | 专项储备(元) | 
 | 78 | surplus_reserve_fund | float | 12 |  |  |  | √ |  | 盈余公积金(元) | 
 | 79 | ordinary_risk_reserve_fund | float | 12 |  |  |  | √ |  | 一般风险准备(元) | 
 | 80 | retained_profit | float | 12 |  |  |  | √ |  | 未分配利润(元) | 
 | 81 | foreign_currency_report_conv_diff | float | 12 |  |  |  | √ |  | 外币报表折算差额(元) | 
 | 82 | equities_parent_company_owners | float | 12 |  |  |  | √ |  | 归属于母公司股东权益合计(元) | 
 | 83 | minority_interests | float | 12 |  |  |  | √ |  | 少数股东权益(元) | 
 | 84 | total_owner_equities | float | 12 |  |  |  | √ |  | 股东权益合计(元) | 
 | 85 | total_sheet_owner_equities | float | 12 |  |  |  | √ |  | 负债和股东权益合计 | 

## stock_daily_cash_flow 股票季度资现金流表

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | date | date |  |  | √ |  |  |  | 日期 | 
 | 2 | code | varchar | 50 |  | √ |  |  |  | 股票代码 | 
 | 3 | pubDate | date |  |  |  |  | √ |  | 公司发布财报日期 | 
 | 4 | statDate | date |  |  |  |  | √ |  | 财报统计的季度的最后一天 | 
 | 5 | goods_sale_and_service_render_cash | float | 12 |  |  |  | √ |  | 销售商品、提供劳务收到的现金(元) | 
 | 6 | net_deposit_increase | float | 12 |  |  |  | √ |  | 客户存款和同业存放款项净增加额(元) | 
 | 7 | net_borrowing_from_central_bank | float | 12 |  |  |  | √ |  | 向中央银行借款净增加额(元) | 
 | 8 | net_borrowing_from_finance_co | float | 12 |  |  |  | √ |  | 向其他金融机构拆入资金净增加额(元) | 
 | 9 | net_original_insurance_cash | float | 12 |  |  |  | √ |  | 收到原保险合同保费取得的现金(元) | 
 | 10 | net_cash_received_from_reinsurance_business | float | 12 |  |  |  | √ |  | 收到再保险业务现金净额(元) | 
 | 11 | net_insurer_deposit_investment | float | 12 |  |  |  | √ |  | 保户储金及投资款净增加额(元) | 
 | 12 | net_deal_trading_assets | float | 12 |  |  |  | √ |  | 处置交易性金融资产净增加额(元) | 
 | 13 | interest_and_commission_cashin | float | 12 |  |  |  | √ |  | 收取利息、手续费及佣金的现金(元) | 
 | 14 | net_increase_in_placements | float | 12 |  |  |  | √ |  | 拆入资金净增加额(元) | 
 | 15 | net_buyback | float | 12 |  |  |  | √ |  | 回购业务资金净增加额(元) | 
 | 16 | tax_levy_refund | float | 12 |  |  |  | √ |  | 收到的税费返还(元) | 
 | 17 | other_cashin_related_operate | float | 12 |  |  |  | √ |  | 收到其他与经营活动有关的现金(元) | 
 | 18 | subtotal_operate_cash_inflow | float | 12 |  |  |  | √ |  | 经营活动现金流入小计(元) | 
 | 19 | goods_and_services_cash_paid | float | 12 |  |  |  | √ |  | 购买商品、接受劳务支付的现金(元) | 
 | 20 | net_loan_and_advance_increase | float | 12 |  |  |  | √ |  | 客户贷款及垫款净增加额(元) | 
 | 21 | net_deposit_in_cb_and_ib | float | 12 |  |  |  | √ |  | 存放中央银行和同业款项净增加额(元) | 
 | 22 | original_compensation_paid | float | 12 |  |  |  | √ |  | 支付原保险合同赔付款项的现金(元) | 
 | 23 | handling_charges_and_commission | float | 12 |  |  |  | √ |  | 支付利息、手续费及佣金的现金(元) | 
 | 24 | policy_dividend_cash_paid | float | 12 |  |  |  | √ |  | 支付保单红利的现金(元) | 
 | 25 | staff_behalf_paid | float | 12 |  |  |  | √ |  | 支付给职工以及为职工支付的现金(元) | 
 | 26 | tax_payments | float | 12 |  |  |  | √ |  | 支付的各项税费(元) | 
 | 27 | other_operate_cash_paid | float | 12 |  |  |  | √ |  | 支付其他与经营活动有关的现金(元) | 
 | 28 | subtotal_operate_cash_outflow | float | 12 |  |  |  | √ |  | 经营活动现金流出小计(元) | 
 | 29 | net_operate_cash_flow | float | 12 |  |  |  | √ |  | 经营活动产生的现金流量净额(元) | 
 | 30 | invest_withdrawal_cash | float | 12 |  |  |  | √ |  | 收回投资收到的现金(元) | 
 | 31 | invest_proceeds | float | 12 |  |  |  | √ |  | 取得投资收益收到的现金(元) | 
 | 32 | fix_intan_other_asset_dispo_cash | float | 12 |  |  |  | √ |  | 处置固定资产、无形资产和其他长期资产收回的现金净额(元) | 
 | 33 | net_cash_deal_subcompany | float | 12 |  |  |  | √ |  | 处置子公司及其他营业单位收到的现金净额(元) | 
 | 34 | other_cash_from_invest_act | float | 12 |  |  |  | √ |  | 收到其他与投资活动有关的现金(元) | 
 | 35 | subtotal_invest_cash_inflow | float | 12 |  |  |  | √ |  | 投资活动现金流入小计(元) | 
 | 36 | fix_intan_other_asset_acqui_cash | float | 12 |  |  |  | √ |  | 购建固定资产、无形资产和其他长期资产支付的现金(元) | 
 | 37 | invest_cash_paid | float | 12 |  |  |  | √ |  | 投资支付的现金(元) | 
 | 38 | impawned_loan_net_increase | float | 12 |  |  |  | √ |  | 质押贷款净增加额(元) | 
 | 39 | net_cash_from_sub_company | float | 12 |  |  |  | √ |  | 取得子公司及其他营业单位支付的现金净额(元) | 
 | 40 | other_cash_to_invest_act | float | 12 |  |  |  | √ |  | 支付其他与投资活动有关的现金(元) | 
 | 41 | subtotal_invest_cash_outflow | float | 12 |  |  |  | √ |  | 投资活动现金流出小计(元) | 
 | 42 | net_invest_cash_flow | float | 12 |  |  |  | √ |  | 投资活动产生的现金流量净额(元) | 
 | 43 | cash_from_invest | float | 12 |  |  |  | √ |  | 吸收投资收到的现金(元) | 
 | 44 | cash_from_mino_s_invest_sub | float | 12 |  |  |  | √ |  | 子公司吸收少数股东投资收到的现金(元) | 
 | 45 | cash_from_borrowing | float | 12 |  |  |  | √ |  | 取得借款收到的现金(元) | 
 | 46 | cash_from_bonds_issue | float | 12 |  |  |  | √ |  | 发行债券收到的现金(元) | 
 | 47 | other_finance_act_cash | float | 12 |  |  |  | √ |  | 收到其他与筹资活动有关的现金(元) | 
 | 48 | subtotal_finance_cash_inflow | float | 12 |  |  |  | √ |  | 筹资活动现金流入小计(元) | 
 | 49 | borrowing_repayment | float | 12 |  |  |  | √ |  | 偿还债务支付的现金(元) | 
 | 50 | dividend_interest_payment | float | 12 |  |  |  | √ |  | 分配股利、利润或偿付利息支付的现金(元) | 
 | 51 | proceeds_from_sub_to_mino_s | float | 12 |  |  |  | √ |  | 子公司支付给少数股东的股利、利润(元) | 
 | 52 | other_finance_act_payment | float | 12 |  |  |  | √ |  | 支付其他与筹资活动有关的现金(元) | 
 | 53 | subtotal_finance_cash_outflow | float | 12 |  |  |  | √ |  | 筹资活动现金流出小计(元) | 
 | 54 | net_finance_cash_flow | float | 12 |  |  |  | √ |  | 筹资活动产生的现金流量净额(元) | 
 | 55 | exchange_rate_change_effect | float | 12 |  |  |  | √ |  | 汇率变动对现金及现金等价物的影响 | 
 | 56 | cash_equivalent_increase | float | 12 |  |  |  | √ |  | 现金及现金等价物净增加额 | 
 | 57 | cash_equivalents_at_beginning | float | 12 |  |  |  | √ |  | 期初现金及现金等价物余额(元) | 
 | 58 | cash_and_equivalents_at_end | float | 12 |  |  |  | √ |  | 期末现金及现金等价物余额(元) | 

## stock_daily_income 股票季度资现金流表

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | date | date |  |  | √ |  |  |  | 日期 | 
 | 2 | code | varchar | 50 |  | √ |  |  |  | 股票代码 | 
 | 3 | pubDate | date |  |  |  |  | √ |  | 公司发布财报日期 | 
 | 4 | statDate | date |  |  |  |  | √ |  | 财报统计的季度的最后一天 | 
 | 5 | total_operating_revenue | float | 12 |  |  |  | √ |  | 营业总收入(元) | 
 | 6 | operating_revenue | float | 12 |  |  |  | √ |  | 营业收入(元) | 
 | 7 | interest_income | float | 12 |  |  |  | √ |  | 利息收入(元) | 
 | 8 | premiums_earned | float | 12 |  |  |  | √ |  | 已赚保费(元) | 
 | 9 | commission_income | float | 12 |  |  |  | √ |  | 手续费及佣金收入(元) | 
 | 10 | total_operating_cost | float | 12 |  |  |  | √ |  | 营业总成本(元) | 
 | 11 | operating_cost | float | 12 |  |  |  | √ |  | 营业成本(元) | 
 | 12 | interest_expense | float | 12 |  |  |  | √ |  | 利息支出(元) | 
 | 13 | commission_expense | float | 12 |  |  |  | √ |  | 手续费及佣金支出(元) | 
 | 14 | refunded_premiums | float | 12 |  |  |  | √ |  | 退保金(元) | 
 | 15 | net_pay_insurance_claims | float | 12 |  |  |  | √ |  | 赔付支出净额(元) | 
 | 16 | withdraw_insurance_contract_reserve | float | 12 |  |  |  | √ |  | 提取保险合同准备金净额(元) | 
 | 17 | policy_dividend_payout | float | 12 |  |  |  | √ |  | 保单红利支出(元) | 
 | 18 | reinsurance_cost | float | 12 |  |  |  | √ |  | 分保费用(元) | 
 | 19 | operating_tax_surcharges | float | 12 |  |  |  | √ |  | 营业税金及附加(元) | 
 | 20 | sale_expense | float | 12 |  |  |  | √ |  | 销售费用(元) | 
 | 21 | administration_expense | float | 12 |  |  |  | √ |  | 管理费用(元) | 
 | 22 | financial_expense | float | 12 |  |  |  | √ |  | 财务费用(元) | 
 | 23 | asset_impairment_loss | float | 12 |  |  |  | √ |  | 资产减值损失(元) | 
 | 24 | fair_value_variable_income | float | 12 |  |  |  | √ |  | 公允价值变动收益(元) | 
 | 25 | investment_income | float | 12 |  |  |  | √ |  | 投资收益(元) | 
 | 26 | invest_income_associates | float | 12 |  |  |  | √ |  | 对联营企业和合营企业的投资收益(元) | 
 | 27 | exchange_income | float | 12 |  |  |  | √ |  | 汇兑收益(元) | 
 | 28 | operating_profit | float | 12 |  |  |  | √ |  | 营业利润(元) | 
 | 29 | non_operating_revenue | float | 12 |  |  |  | √ |  | 营业外收入(元) | 
 | 30 | non_operating_expense | float | 12 |  |  |  | √ |  | 营业外支出(元) | 
 | 31 | disposal_loss_non_current_liability | float | 12 |  |  |  | √ |  | 非流动资产处置净损失(元) | 
 | 32 | total_profit | float | 12 |  |  |  | √ |  | 利润总额(元) | 
 | 33 | income_tax_expense | float | 12 |  |  |  | √ |  | 所得税费用(元) | 
 | 34 | net_profit | float | 12 |  |  |  | √ |  | 净利润(元) | 
 | 35 | np_parent_company_owners | float | 12 |  |  |  | √ |  | 归属于母公司股东的净利润(元) | 
 | 36 | minority_profit | float | 12 |  |  |  | √ |  | 少数股东损益(元) | 
 | 37 | basic_eps | float | 12 |  |  |  | √ |  | 基本每股收益(元) | 
 | 38 | diluted_eps | float | 12 |  |  |  | √ |  | 稀释每股收益(元) | 
 | 39 | other_composite_income | float | 12 |  |  |  | √ |  | 其他综合收益(元) | 
 | 40 | total_composite_income | float | 12 |  |  |  | √ |  | 综合收益总额(元) | 
 | 41 | ci_parent_company_owners | float | 12 |  |  |  | √ |  | 归属于母公司所有者的综合收益总额(元) | 
 | 42 | ci_minority_owners | float | 12 |  |  |  | √ |  | 归属于少数股东的综合收益总额(元) | 

## stock_daily_indicator 股票每日市值相关指标

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | date | date |  |  | √ |  |  |  | 日期 | 
 | 2 | code | varchar | 50 |  | √ |  |  |  | 股票代码 | 
 | 3 | capitalization | float | 12 |  |  |  | √ |  | 总股本(万股) | 
 | 4 | circulating_cap | float | 12 |  |  |  | √ |  | 流通股本(万股) | 
 | 5 | market_cap | float | 12 |  |  |  | √ |  | 总市值(亿元) | 
 | 6 | circulating_market_cap | float | 12 |  |  |  | √ |  | 流通市值(亿元) | 
 | 7 | turnover_ratio | float | 12 |  |  |  | √ |  | 换手率(%) | 
 | 8 | pe_ratio | float | 12 |  |  |  | √ |  | 市盈率(PE, TTM) | 
 | 9 | pe_ratio_lyr | float | 12 |  |  |  | √ |  | 市盈率(PE) | 
 | 10 | pb_ratio | float | 12 |  |  |  | √ |  | 市净率(PB) | 
 | 11 | ps_ratio | float | 12 |  |  |  | √ |  | 市销率(PS, TTM) | 
 | 12 | pcf_ratio | float | 12 |  |  |  | √ |  | 市现率(PCF, 现金净流量TTM) | 

## stock_daily_industry 股票每日所属行业

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | date | date |  |  | √ |  |  |  | 日期 | 
 | 2 | code | varchar | 50 |  | √ |  |  |  | 股票代码 | 
 | 3 | jq_l1 | varchar | 50 |  |  |  | √ |  | 聚宽一级行业 | 
 | 4 | jq_l2 | varchar | 50 |  |  |  | √ |  | 聚宽二级行业 | 
 | 5 | sw_l1 | varchar | 50 |  |  |  | √ |  | 申万一级行业 | 
 | 6 | sw_l2 | varchar | 50 |  |  |  | √ |  | 申万二级行业 | 
 | 7 | sw_l3 | varchar | 50 |  |  |  | √ |  | 申万三级行业 | 
 | 8 | zjw | varchar | 50 |  |  |  | √ |  | 证监会行业 | 

## stock_daily_price 股票每日行情--价格不复权

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | date | date |  |  | √ |  |  |  | 日期 | 
 | 2 | code | varchar | 50 |  | √ |  |  |  | 股票代码 | 
 | 3 | open | float | 12 |  |  |  | √ |  | 开盘价 | 
 | 4 | close | float | 12 |  |  |  | √ |  | 收盘价 | 
 | 5 | low | float | 12 |  |  |  | √ |  | 最低价 | 
 | 6 | high | float | 12 |  |  |  | √ |  | 最高价 | 
 | 7 | volume | float | 12 |  |  |  | √ |  | 成交量 | 
 | 8 | money | float | 12 |  |  |  | √ |  | 成交额 | 
 | 9 | factor | float | 12 |  |  |  | √ |  | 复权因子 | 
 | 10 | high_limit | float | 12 |  |  |  | √ |  | 涨停价 | 
 | 11 | low_limit | float | 12 |  |  |  | √ |  | 跌停价 | 
 | 12 | vwap | float | 12 |  |  |  | √ |  | 成交量加权均价 | 
 | 13 | pre_close | float | 12 |  |  |  | √ |  | 昨日收盘价 | 
 | 14 | paused | tinyint |  | 0 |  |  | √ |  | 是否停牌 | 

## stock_daily_price_post 股票每日行情--价格后复权

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | date | date |  |  | √ |  |  |  | 日期 | 
 | 2 | code | varchar | 50 |  | √ |  |  |  | 股票代码 | 
 | 3 | open | float | 12 |  |  |  | √ |  | 开盘价 | 
 | 4 | close | float | 12 |  |  |  | √ |  | 收盘价 | 
 | 5 | low | float | 12 |  |  |  | √ |  | 最低价 | 
 | 6 | high | float | 12 |  |  |  | √ |  | 最高价 | 
 | 7 | volume | float | 12 |  |  |  | √ |  | 成交量 | 
 | 8 | money | float | 12 |  |  |  | √ |  | 成交额 | 
 | 9 | factor | float | 12 |  |  |  | √ |  | 复权因子 | 
 | 10 | high_limit | float | 12 |  |  |  | √ |  | 涨停价 | 
 | 11 | low_limit | float | 12 |  |  |  | √ |  | 跌停价 | 
 | 12 | vwap | float | 12 |  |  |  | √ |  | 成交量加权均价 | 
 | 13 | pre_close | float | 12 |  |  |  | √ |  | 昨日收盘价 | 
 | 14 | paused | tinyint |  | 0 |  |  | √ |  | 是否停牌 | 

## stock_is_st 股票每日是否st

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | date | date |  |  | √ |  |  |  | 日期 | 
 | 2 | code | varchar | 50 |  | √ |  |  |  | 股票代码 | 
 | 3 | is_st | tinyint |  | 0 |  |  | √ |  | 是否st,*st和退市整理期标的 | 

## trade_days 获取 A 股市场交易日日期

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | trade_date | date |  |  | √ |  |  |  | 交易日期 | 

# 1_ods_tushare

## index_basic 获取指数基础信息

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | ts_code | varchar | 255 |  | √ |  |  |  | TS代码 | 
 | 2 | name | varchar | 255 |  |  |  | √ |  | 简称 | 
 | 3 | fullname | varchar | 255 |  |  |  | √ |  | 指数全称 | 
 | 4 | market | varchar | 255 |  |  |  | √ |  | 市场 | 
 | 5 | publisher | varchar | 255 |  |  |  | √ |  | 发布方 | 
 | 6 | index_type | varchar | 255 |  |  |  | √ |  | 指数风格 | 
 | 7 | category | varchar | 255 |  |  |  | √ |  | 指数类别 | 
 | 8 | base_date | date |  |  |  |  | √ |  | 基期 | 
 | 9 | base_point | float | 12 |  |  |  | √ |  | 基点 | 
 | 10 | list_date | date |  |  |  |  | √ |  | 发布日期 | 
 | 11 | weight_rule | varchar | 255 |  |  |  | √ |  | 加权方式 | 
 | 12 | desc | text | 65535 |  |  |  | √ |  | 描述 | 
 | 13 | exp_date | date |  |  |  |  | √ |  | 终止日期 | 

## index_weight 获取各类指数成分和权重，月度数据

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | trade_date | date |  |  | √ |  |  |  | 交易日期 | 
 | 2 | index_code | varchar | 50 |  | √ |  |  |  | 指数代码 | 
 | 3 | con_code | varchar | 50 |  | √ |  |  |  | 成分代码 | 
 | 4 | weight | float | 12 |  |  |  | √ |  | 权重 | 

## stock_balancesheet 获取上市公司资产负债表

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | f_ann_date | date |  |  | √ |  |  |  | 实际公告日期 | 
 | 2 | ts_code | varchar | 50 |  | √ |  |  |  | TS代码 | 
 | 3 | ann_date | date |  |  |  |  | √ |  | 公告日期 | 
 | 4 | end_date | date |  |  | √ |  |  |  | 报告期 | 
 | 5 | report_type | float | 12 |  | √ |  |  |  | 报告类型 1合并报表 2单季合并 3调整单季合并表 4调整合并报表 5调整前合并报表 6母公司报表 7母公司单季表 8 母公司调整单季表 9母公司调整表 10母公司调整前报表 11调整前合并报表 12母公司调整前报表 | 
 | 6 | comp_type | float | 12 |  |  |  | √ |  | 公司类型(1一般工商业2银行3保险4证券) | 
 | 7 | total_share | float | 12 |  |  |  | √ |  | 期末总股本 | 
 | 8 | cap_rese | float | 12 |  |  |  | √ |  | 资本公积金 | 
 | 9 | undistr_porfit | float | 12 |  |  |  | √ |  | 未分配利润 | 
 | 10 | surplus_rese | float | 12 |  |  |  | √ |  | 盈余公积金 | 
 | 11 | special_rese | float | 12 |  |  |  | √ |  | 专项储备 | 
 | 12 | money_cap | float | 12 |  |  |  | √ |  | 货币资金 | 
 | 13 | trad_asset | float | 12 |  |  |  | √ |  | 交易性金融资产 | 
 | 14 | notes_receiv | float | 12 |  |  |  | √ |  | 应收票据 | 
 | 15 | accounts_receiv | float | 12 |  |  |  | √ |  | 应收账款 | 
 | 16 | oth_receiv | float | 12 |  |  |  | √ |  | 其他应收款 | 
 | 17 | prepayment | float | 12 |  |  |  | √ |  | 预付款项 | 
 | 18 | div_receiv | float | 12 |  |  |  | √ |  | 应收股利 | 
 | 19 | int_receiv | float | 12 |  |  |  | √ |  | 应收利息 | 
 | 20 | inventories | float | 12 |  |  |  | √ |  | 存货 | 
 | 21 | amor_exp | float | 12 |  |  |  | √ |  | 长期待摊费用 | 
 | 22 | nca_within_1y | float | 12 |  |  |  | √ |  | 一年内到期的非流动资产 | 
 | 23 | sett_rsrv | float | 12 |  |  |  | √ |  | 结算备付金 | 
 | 24 | loanto_oth_bank_fi | float | 12 |  |  |  | √ |  | 拆出资金 | 
 | 25 | premium_receiv | float | 12 |  |  |  | √ |  | 应收保费 | 
 | 26 | reinsur_receiv | float | 12 |  |  |  | √ |  | 应收分保账款 | 
 | 27 | reinsur_res_receiv | float | 12 |  |  |  | √ |  | 应收分保合同准备金 | 
 | 28 | pur_resale_fa | float | 12 |  |  |  | √ |  | 买入返售金融资产 | 
 | 29 | oth_cur_assets | float | 12 |  |  |  | √ |  | 其他流动资产 | 
 | 30 | total_cur_assets | float | 12 |  |  |  | √ |  | 流动资产合计 | 
 | 31 | fa_avail_for_sale | float | 12 |  |  |  | √ |  | 可供出售金融资产 | 
 | 32 | htm_invest | float | 12 |  |  |  | √ |  | 持有至到期投资 | 
 | 33 | lt_eqt_invest | float | 12 |  |  |  | √ |  | 长期股权投资 | 
 | 34 | invest_real_estate | float | 12 |  |  |  | √ |  | 投资性房地产 | 
 | 35 | time_deposits | float | 12 |  |  |  | √ |  | 定期存款 | 
 | 36 | oth_assets | float | 12 |  |  |  | √ |  | 其他资产 | 
 | 37 | lt_rec | float | 12 |  |  |  | √ |  | 长期应收款 | 
 | 38 | fix_assets | float | 12 |  |  |  | √ |  | 固定资产 | 
 | 39 | cip | float | 12 |  |  |  | √ |  | 在建工程 | 
 | 40 | const_materials | float | 12 |  |  |  | √ |  | 工程物资 | 
 | 41 | fixed_assets_disp | float | 12 |  |  |  | √ |  | 固定资产清理 | 
 | 42 | produc_bio_assets | float | 12 |  |  |  | √ |  | 生产性生物资产 | 
 | 43 | oil_and_gas_assets | float | 12 |  |  |  | √ |  | 油气资产 | 
 | 44 | intan_assets | float | 12 |  |  |  | √ |  | 无形资产 | 
 | 45 | r_and_d | float | 12 |  |  |  | √ |  | 研发支出 | 
 | 46 | goodwill | float | 12 |  |  |  | √ |  | 商誉 | 
 | 47 | lt_amor_exp | float | 12 |  |  |  | √ |  | 长期待摊费用 | 
 | 48 | defer_tax_assets | float | 12 |  |  |  | √ |  | 递延所得税资产 | 
 | 49 | decr_in_disbur | float | 12 |  |  |  | √ |  | 发放贷款及垫款 | 
 | 50 | oth_nca | float | 12 |  |  |  | √ |  | 其他非流动资产 | 
 | 51 | total_nca | float | 12 |  |  |  | √ |  | 非流动资产合计 | 
 | 52 | cash_reser_cb | float | 12 |  |  |  | √ |  | 现金及存放中央银行款项 | 
 | 53 | depos_in_oth_bfi | float | 12 |  |  |  | √ |  | 存放同业和其它金融机构款项 | 
 | 54 | prec_metals | float | 12 |  |  |  | √ |  | 贵金属 | 
 | 55 | deriv_assets | float | 12 |  |  |  | √ |  | 衍生金融资产 | 
 | 56 | rr_reins_une_prem | float | 12 |  |  |  | √ |  | 应收分保未到期责任准备金 | 
 | 57 | rr_reins_outstd_cla | float | 12 |  |  |  | √ |  | 应收分保未决赔款准备金 | 
 | 58 | rr_reins_lins_liab | float | 12 |  |  |  | √ |  | 应收分保寿险责任准备金 | 
 | 59 | rr_reins_lthins_liab | float | 12 |  |  |  | √ |  | 应收分保长期健康险责任准备金 | 
 | 60 | refund_depos | float | 12 |  |  |  | √ |  | 存出保证金 | 
 | 61 | ph_pledge_loans | float | 12 |  |  |  | √ |  | 保户质押贷款 | 
 | 62 | refund_cap_depos | float | 12 |  |  |  | √ |  | 存出资本保证金 | 
 | 63 | indep_acct_assets | float | 12 |  |  |  | √ |  | 独立账户资产 | 
 | 64 | client_depos | float | 12 |  |  |  | √ |  | 其中：客户资金存款 | 
 | 65 | client_prov | float | 12 |  |  |  | √ |  | 其中：客户备付金 | 
 | 66 | transac_seat_fee | float | 12 |  |  |  | √ |  | 其中:交易席位费 | 
 | 67 | invest_as_receiv | float | 12 |  |  |  | √ |  | 应收款项类投资 | 
 | 68 | total_assets | float | 12 |  |  |  | √ |  | 资产总计 | 
 | 69 | lt_borr | float | 12 |  |  |  | √ |  | 长期借款 | 
 | 70 | st_borr | float | 12 |  |  |  | √ |  | 短期借款 | 
 | 71 | cb_borr | float | 12 |  |  |  | √ |  | 向中央银行借款 | 
 | 72 | depos_ib_deposits | float | 12 |  |  |  | √ |  | 吸收存款及同业存放 | 
 | 73 | loan_oth_bank | float | 12 |  |  |  | √ |  | 拆入资金 | 
 | 74 | trading_fl | float | 12 |  |  |  | √ |  | 交易性金融负债 | 
 | 75 | notes_payable | float | 12 |  |  |  | √ |  | 应付票据 | 
 | 76 | acct_payable | float | 12 |  |  |  | √ |  | 应付账款 | 
 | 77 | adv_receipts | float | 12 |  |  |  | √ |  | 预收款项 | 
 | 78 | sold_for_repur_fa | float | 12 |  |  |  | √ |  | 卖出回购金融资产款 | 
 | 79 | comm_payable | float | 12 |  |  |  | √ |  | 应付手续费及佣金 | 
 | 80 | payroll_payable | float | 12 |  |  |  | √ |  | 应付职工薪酬 | 
 | 81 | taxes_payable | float | 12 |  |  |  | √ |  | 应交税费 | 
 | 82 | int_payable | float | 12 |  |  |  | √ |  | 应付利息 | 
 | 83 | div_payable | float | 12 |  |  |  | √ |  | 应付股利 | 
 | 84 | oth_payable | float | 12 |  |  |  | √ |  | 其他应付款 | 
 | 85 | acc_exp | float | 12 |  |  |  | √ |  | 预提费用 | 
 | 86 | deferred_inc | float | 12 |  |  |  | √ |  | 递延收益 | 
 | 87 | st_bonds_payable | float | 12 |  |  |  | √ |  | 应付短期债券 | 
 | 88 | payable_to_reinsurer | float | 12 |  |  |  | √ |  | 应付分保账款 | 
 | 89 | rsrv_insur_cont | float | 12 |  |  |  | √ |  | 保险合同准备金 | 
 | 90 | acting_trading_sec | float | 12 |  |  |  | √ |  | 代理买卖证券款 | 
 | 91 | acting_uw_sec | float | 12 |  |  |  | √ |  | 代理承销证券款 | 
 | 92 | non_cur_liab_due_1y | float | 12 |  |  |  | √ |  | 一年内到期的非流动负债 | 
 | 93 | oth_cur_liab | float | 12 |  |  |  | √ |  | 其他流动负债 | 
 | 94 | total_cur_liab | float | 12 |  |  |  | √ |  | 流动负债合计 | 
 | 95 | bond_payable | float | 12 |  |  |  | √ |  | 应付债券 | 
 | 96 | lt_payable | float | 12 |  |  |  | √ |  | 长期应付款 | 
 | 97 | specific_payables | float | 12 |  |  |  | √ |  | 专项应付款 | 
 | 98 | estimated_liab | float | 12 |  |  |  | √ |  | 预计负债 | 
 | 99 | defer_tax_liab | float | 12 |  |  |  | √ |  | 递延所得税负债 | 
 | 100 | defer_inc_non_cur_liab | float | 12 |  |  |  | √ |  | 递延收益-非流动负债 | 
 | 101 | oth_ncl | float | 12 |  |  |  | √ |  | 其他非流动负债 | 
 | 102 | total_ncl | float | 12 |  |  |  | √ |  | 非流动负债合计 | 
 | 103 | depos_oth_bfi | float | 12 |  |  |  | √ |  | 同业和其它金融机构存放款项 | 
 | 104 | deriv_liab | float | 12 |  |  |  | √ |  | 衍生金融负债 | 
 | 105 | depos | float | 12 |  |  |  | √ |  | 吸收存款 | 
 | 106 | agency_bus_liab | float | 12 |  |  |  | √ |  | 代理业务负债 | 
 | 107 | oth_liab | float | 12 |  |  |  | √ |  | 其他负债 | 
 | 108 | prem_receiv_adva | float | 12 |  |  |  | √ |  | 预收保费 | 
 | 109 | depos_received | float | 12 |  |  |  | √ |  | 存入保证金 | 
 | 110 | ph_invest | float | 12 |  |  |  | √ |  | 保户储金及投资款 | 
 | 111 | reser_une_prem | float | 12 |  |  |  | √ |  | 未到期责任准备金 | 
 | 112 | reser_outstd_claims | float | 12 |  |  |  | √ |  | 未决赔款准备金 | 
 | 113 | reser_lins_liab | float | 12 |  |  |  | √ |  | 寿险责任准备金 | 
 | 114 | reser_lthins_liab | float | 12 |  |  |  | √ |  | 长期健康险责任准备金 | 
 | 115 | indept_acc_liab | float | 12 |  |  |  | √ |  | 独立账户负债 | 
 | 116 | pledge_borr | float | 12 |  |  |  | √ |  | 其中:质押借款 | 
 | 117 | indem_payable | float | 12 |  |  |  | √ |  | 应付赔付款 | 
 | 118 | policy_div_payable | float | 12 |  |  |  | √ |  | 应付保单红利 | 
 | 119 | total_liab | float | 12 |  |  |  | √ |  | 负债合计 | 
 | 120 | treasury_share | float | 12 |  |  |  | √ |  | 减:库存股 | 
 | 121 | ordin_risk_reser | float | 12 |  |  |  | √ |  | 一般风险准备 | 
 | 122 | forex_differ | float | 12 |  |  |  | √ |  | 外币报表折算差额 | 
 | 123 | invest_loss_unconf | float | 12 |  |  |  | √ |  | 未确认的投资损失 | 
 | 124 | minority_int | float | 12 |  |  |  | √ |  | 少数股东权益 | 
 | 125 | total_hldr_eqy_exc_min_int | float | 12 |  |  |  | √ |  | 股东权益合计(不含少数股东权益) | 
 | 126 | total_hldr_eqy_inc_min_int | float | 12 |  |  |  | √ |  | 股东权益合计(含少数股东权益) | 
 | 127 | total_liab_hldr_eqy | float | 12 |  |  |  | √ |  | 负债及股东权益总计 | 
 | 128 | lt_payroll_payable | float | 12 |  |  |  | √ |  | 长期应付职工薪酬 | 
 | 129 | oth_comp_income | float | 12 |  |  |  | √ |  | 其他综合收益 | 
 | 130 | oth_eqt_tools | float | 12 |  |  |  | √ |  | 其他权益工具 | 
 | 131 | oth_eqt_tools_p_shr | float | 12 |  |  |  | √ |  | 其他权益工具(优先股) | 
 | 132 | lending_funds | float | 12 |  |  |  | √ |  | 融出资金 | 
 | 133 | acc_receivable | float | 12 |  |  |  | √ |  | 应收款项 | 
 | 134 | st_fin_payable | float | 12 |  |  |  | √ |  | 应付短期融资款 | 
 | 135 | payables | float | 12 |  |  |  | √ |  | 应付款项 | 
 | 136 | hfs_assets | float | 12 |  |  |  | √ |  | 持有待售的资产 | 
 | 137 | hfs_sales | float | 12 |  |  |  | √ |  | 持有待售的负债 | 

## stock_cashflow 获取上市公司现金流量表

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | f_ann_date | date |  |  | √ |  |  |  | 实际公告日期 | 
 | 2 | ts_code | varchar | 50 |  | √ |  |  |  | TS代码 | 
 | 3 | ann_date | date |  |  |  |  | √ |  | 公告日期 | 
 | 4 | end_date | date |  |  | √ |  |  |  | 报告期 | 
 | 5 | report_type | float | 12 |  | √ |  |  |  | 报告类型 1合并报表 2单季合并 3调整单季合并表 4调整合并报表 5调整前合并报表 6母公司报表 7母公司单季表 8 母公司调整单季表 9母公司调整表 10母公司调整前报表 11调整前合并报表 12母公司调整前报表 | 
 | 6 | comp_type | float | 12 |  |  |  | √ |  | 公司类型(1一般工商业2银行3保险4证券) | 
 | 7 | net_profit | float | 12 |  |  |  | √ |  | 净利润 | 
 | 8 | finan_exp | float | 12 |  |  |  | √ |  | 财务费用 | 
 | 9 | c_fr_sale_sg | float | 12 |  |  |  | √ |  | 销售商品、提供劳务收到的现金 | 
 | 10 | recp_tax_rends | float | 12 |  |  |  | √ |  | 收到的税费返还 | 
 | 11 | n_depos_incr_fi | float | 12 |  |  |  | √ |  | 客户存款和同业存放款项净增加额 | 
 | 12 | n_incr_loans_cb | float | 12 |  |  |  | √ |  | 向中央银行借款净增加额 | 
 | 13 | n_inc_borr_oth_fi | float | 12 |  |  |  | √ |  | 向其他金融机构拆入资金净增加额 | 
 | 14 | prem_fr_orig_contr | float | 12 |  |  |  | √ |  | 收到原保险合同保费取得的现金 | 
 | 15 | n_incr_insured_dep | float | 12 |  |  |  | √ |  | 保户储金净增加额 | 
 | 16 | n_reinsur_prem | float | 12 |  |  |  | √ |  | 收到再保业务现金净额 | 
 | 17 | n_incr_disp_tfa | float | 12 |  |  |  | √ |  | 处置交易性金融资产净增加额 | 
 | 18 | ifc_cash_incr | float | 12 |  |  |  | √ |  | 收取利息和手续费净增加额 | 
 | 19 | n_incr_disp_faas | float | 12 |  |  |  | √ |  | 处置可供出售金融资产净增加额 | 
 | 20 | n_incr_loans_oth_bank | float | 12 |  |  |  | √ |  | 拆入资金净增加额 | 
 | 21 | n_cap_incr_repur | float | 12 |  |  |  | √ |  | 回购业务资金净增加额 | 
 | 22 | c_fr_oth_operate_a | float | 12 |  |  |  | √ |  | 收到其他与经营活动有关的现金 | 
 | 23 | c_inf_fr_operate_a | float | 12 |  |  |  | √ |  | 经营活动现金流入小计 | 
 | 24 | c_paid_goods_s | float | 12 |  |  |  | √ |  | 购买商品、接受劳务支付的现金 | 
 | 25 | c_paid_to_for_empl | float | 12 |  |  |  | √ |  | 支付给职工以及为职工支付的现金 | 
 | 26 | c_paid_for_taxes | float | 12 |  |  |  | √ |  | 支付的各项税费 | 
 | 27 | n_incr_clt_loan_adv | float | 12 |  |  |  | √ |  | 客户贷款及垫款净增加额 | 
 | 28 | n_incr_dep_cbob | float | 12 |  |  |  | √ |  | 存放央行和同业款项净增加额 | 
 | 29 | c_pay_claims_orig_inco | float | 12 |  |  |  | √ |  | 支付原保险合同赔付款项的现金 | 
 | 30 | pay_handling_chrg | float | 12 |  |  |  | √ |  | 支付手续费的现金 | 
 | 31 | pay_comm_insur_plcy | float | 12 |  |  |  | √ |  | 支付保单红利的现金 | 
 | 32 | oth_cash_pay_oper_act | float | 12 |  |  |  | √ |  | 支付其他与经营活动有关的现金 | 
 | 33 | st_cash_out_act | float | 12 |  |  |  | √ |  | 经营活动现金流出小计 | 
 | 34 | n_cashflow_act | float | 12 |  |  |  | √ |  | 经营活动产生的现金流量净额 | 
 | 35 | oth_recp_ral_inv_act | float | 12 |  |  |  | √ |  | 收到其他与投资活动有关的现金 | 
 | 36 | c_disp_withdrwl_invest | float | 12 |  |  |  | √ |  | 收回投资收到的现金 | 
 | 37 | c_recp_return_invest | float | 12 |  |  |  | √ |  | 取得投资收益收到的现金 | 
 | 38 | n_recp_disp_fiolta | float | 12 |  |  |  | √ |  | 处置固定资产、无形资产和其他长期资产收回的现金净额 | 
 | 39 | n_recp_disp_sobu | float | 12 |  |  |  | √ |  | 处置子公司及其他营业单位收到的现金净额 | 
 | 40 | stot_inflows_inv_act | float | 12 |  |  |  | √ |  | 投资活动现金流入小计 | 
 | 41 | c_pay_acq_const_fiolta | float | 12 |  |  |  | √ |  | 购建固定资产、无形资产和其他长期资产支付的现金 | 
 | 42 | c_paid_invest | float | 12 |  |  |  | √ |  | 投资支付的现金 | 
 | 43 | n_disp_subs_oth_biz | float | 12 |  |  |  | √ |  | 取得子公司及其他营业单位支付的现金净额 | 
 | 44 | oth_pay_ral_inv_act | float | 12 |  |  |  | √ |  | 支付其他与投资活动有关的现金 | 
 | 45 | n_incr_pledge_loan | float | 12 |  |  |  | √ |  | 质押贷款净增加额 | 
 | 46 | stot_out_inv_act | float | 12 |  |  |  | √ |  | 投资活动现金流出小计 | 
 | 47 | n_cashflow_inv_act | float | 12 |  |  |  | √ |  | 投资活动产生的现金流量净额 | 
 | 48 | c_recp_borrow | float | 12 |  |  |  | √ |  | 取得借款收到的现金 | 
 | 49 | proc_issue_bonds | float | 12 |  |  |  | √ |  | 发行债券收到的现金 | 
 | 50 | oth_cash_recp_ral_fnc_act | float | 12 |  |  |  | √ |  | 收到其他与筹资活动有关的现金 | 
 | 51 | stot_cash_in_fnc_act | float | 12 |  |  |  | √ |  | 筹资活动现金流入小计 | 
 | 52 | free_cashflow | float | 12 |  |  |  | √ |  | 企业自由现金流量 | 
 | 53 | c_prepay_amt_borr | float | 12 |  |  |  | √ |  | 偿还债务支付的现金 | 
 | 54 | c_pay_dist_dpcp_int_exp | float | 12 |  |  |  | √ |  | 分配股利、利润或偿付利息支付的现金 | 
 | 55 | incl_dvd_profit_paid_sc_ms | float | 12 |  |  |  | √ |  | 其中:子公司支付给少数股东的股利、利润 | 
 | 56 | oth_cashpay_ral_fnc_act | float | 12 |  |  |  | √ |  | 支付其他与筹资活动有关的现金 | 
 | 57 | stot_cashout_fnc_act | float | 12 |  |  |  | √ |  | 筹资活动现金流出小计 | 
 | 58 | n_cash_flows_fnc_act | float | 12 |  |  |  | √ |  | 筹资活动产生的现金流量净额 | 
 | 59 | eff_fx_flu_cash | float | 12 |  |  |  | √ |  | 汇率变动对现金的影响 | 
 | 60 | n_incr_cash_cash_equ | float | 12 |  |  |  | √ |  | 现金及现金等价物净增加额 | 
 | 61 | c_cash_equ_beg_period | float | 12 |  |  |  | √ |  | 期初现金及现金等价物余额 | 
 | 62 | c_cash_equ_end_period | float | 12 |  |  |  | √ |  | 期末现金及现金等价物余额 | 
 | 63 | c_recp_cap_contrib | float | 12 |  |  |  | √ |  | 吸收投资收到的现金 | 
 | 64 | incl_cash_rec_saims | float | 12 |  |  |  | √ |  | 其中:子公司吸收少数股东投资收到的现金 | 
 | 65 | uncon_invest_loss | float | 12 |  |  |  | √ |  | 未确认投资损失 | 
 | 66 | prov_depr_assets | float | 12 |  |  |  | √ |  | 加:资产减值准备 | 
 | 67 | depr_fa_coga_dpba | float | 12 |  |  |  | √ |  | 固定资产折旧、油气资产折耗、生产性生物资产折旧 | 
 | 68 | amort_intang_assets | float | 12 |  |  |  | √ |  | 无形资产摊销 | 
 | 69 | lt_amort_deferred_exp | float | 12 |  |  |  | √ |  | 长期待摊费用摊销 | 
 | 70 | decr_deferred_exp | float | 12 |  |  |  | √ |  | 待摊费用减少 | 
 | 71 | incr_acc_exp | float | 12 |  |  |  | √ |  | 预提费用增加 | 
 | 72 | loss_disp_fiolta | float | 12 |  |  |  | √ |  | 处置固定、无形资产和其他长期资产的损失 | 
 | 73 | loss_scr_fa | float | 12 |  |  |  | √ |  | 固定资产报废损失 | 
 | 74 | loss_fv_chg | float | 12 |  |  |  | √ |  | 公允价值变动损失 | 
 | 75 | invest_loss | float | 12 |  |  |  | √ |  | 投资损失 | 
 | 76 | decr_def_inc_tax_assets | float | 12 |  |  |  | √ |  | 递延所得税资产减少 | 
 | 77 | incr_def_inc_tax_liab | float | 12 |  |  |  | √ |  | 递延所得税负债增加 | 
 | 78 | decr_inventories | float | 12 |  |  |  | √ |  | 存货的减少 | 
 | 79 | decr_oper_payable | float | 12 |  |  |  | √ |  | 经营性应收项目的减少 | 
 | 80 | incr_oper_payable | float | 12 |  |  |  | √ |  | 经营性应付项目的增加 | 
 | 81 | others | float | 12 |  |  |  | √ |  | 其他 | 
 | 82 | im_net_cashflow_oper_act | float | 12 |  |  |  | √ |  | 经营活动产生的现金流量净额(间接法) | 
 | 83 | conv_debt_into_cap | float | 12 |  |  |  | √ |  | 债务转为资本 | 
 | 84 | conv_copbonds_due_within_1y | float | 12 |  |  |  | √ |  | 一年内到期的可转换公司债券 | 
 | 85 | fa_fnc_leases | float | 12 |  |  |  | √ |  | 融资租入固定资产 | 
 | 86 | end_bal_cash | float | 12 |  |  |  | √ |  | 现金的期末余额 | 
 | 87 | beg_bal_cash | float | 12 |  |  |  | √ |  | 减:现金的期初余额 | 
 | 88 | end_bal_cash_equ | float | 12 |  |  |  | √ |  | 加:现金等价物的期末余额 | 
 | 89 | beg_bal_cash_equ | float | 12 |  |  |  | √ |  | 减:现金等价物的期初余额 | 
 | 90 | im_n_incr_cash_equ | float | 12 |  |  |  | √ |  | 现金及现金等价物净增加额(间接法) | 

## stock_company 获取上市公司基础信息

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | ts_code | varchar | 255 |  | √ |  |  |  | 股票代码 | 
 | 2 | exchange | varchar | 255 |  |  |  | √ |  | 交易所代码SSE上交所 SZSE深交所 | 
 | 3 | chairman | varchar | 255 |  |  |  | √ |  | 法人代表 | 
 | 4 | manager | varchar | 255 |  |  |  | √ |  | 总经理 | 
 | 5 | secretary | varchar | 255 |  |  |  | √ |  | 董秘 | 
 | 6 | reg_capital | float | 12 |  |  |  | √ |  | 注册资本 | 
 | 7 | setup_date | date |  |  |  |  | √ |  | 注册日期 | 
 | 8 | province | varchar | 255 |  |  |  | √ |  | 所在省份 | 
 | 9 | city | varchar | 255 |  |  |  | √ |  | 所在城市 | 
 | 10 | introduction | text | 65535 |  |  |  | √ |  | 公司介绍 | 
 | 11 | website | varchar | 255 |  |  |  | √ |  | 公司主页 | 
 | 12 | email | varchar | 255 |  |  |  | √ |  | 电子邮件 | 
 | 13 | office | varchar | 255 |  |  |  | √ |  | 办公室 | 
 | 14 | ann_date | date |  |  |  |  | √ |  | 公告日期 | 
 | 15 | business_scope | text | 65535 |  |  |  | √ |  | 经营范围 | 
 | 16 | employees | int |  |  |  |  | √ |  | 员工人数 | 
 | 17 | main_business | text | 65535 |  |  |  | √ |  | 主要业务及产品 | 

## stock_dividend 获取上市公司分红送股数据

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | ann_date | date |  |  | √ |  |  |  | 预案公告日（董事会） | 
 | 2 | ts_code | varchar | 50 |  | √ |  |  |  | TS代码 | 
 | 3 | end_date | date |  |  | √ |  |  |  | 分送年度 | 
 | 4 | div_proc | varchar | 255 |  | √ |  |  |  | 实施进度 | 
 | 5 | stk_div | float | 12 |  |  |  | √ |  | 每股送转 | 
 | 6 | stk_bo_rate | float | 12 |  |  |  | √ |  | 每股送股比例 | 
 | 7 | stk_co_rate | float | 12 |  |  |  | √ |  | 每股转增比例 | 
 | 8 | cash_div | float | 12 |  |  |  | √ |  | 每股分红（税后） | 
 | 9 | cash_div_tax | float | 12 |  |  |  | √ |  | 每股分红（税前） | 
 | 10 | record_date | date |  |  |  |  | √ |  | 股权登记日 | 
 | 11 | ex_date | date |  |  |  |  | √ |  | 除权除息日 | 
 | 12 | pay_date | date |  |  |  |  | √ |  | 派息日 | 
 | 13 | div_listdate | date |  |  |  |  | √ |  | 红股上市日 | 
 | 14 | imp_ann_date | date |  |  |  |  | √ |  | 实施公告日 | 
 | 15 | base_date | date |  |  |  |  | √ |  | 基准日 | 
 | 16 | base_share | float | 12 |  |  |  | √ |  | 实施基准股本（万） | 
 | 17 | update_flag | float | 12 |  |  |  | √ |  | 是否变更过（1表示变更） | 

## stock_express 获取上市公司业绩快报

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | ann_date | date |  |  | √ |  |  |  | 公告日期 | 
 | 2 | ts_code | varchar | 50 |  | √ |  |  |  | TS代码 | 
 | 3 | end_date | date |  |  | √ |  |  |  | 报告期 | 
 | 4 | revenue | float | 12 |  |  |  | √ |  | 营业收入(元) | 
 | 5 | operate_profit | float | 12 |  |  |  | √ |  | 营业利润(元) | 
 | 6 | total_profit | float | 12 |  |  |  | √ |  | 利润总额(元) | 
 | 7 | n_income | float | 12 |  |  |  | √ |  | 净利润(元) | 
 | 8 | total_assets | float | 12 |  |  |  | √ |  | 总资产(元) | 
 | 9 | total_hldr_eqy_exc_min_int | float | 12 |  |  |  | √ |  | 股东权益合计(不含少数股东权益)(元) | 
 | 10 | diluted_eps | float | 12 |  |  |  | √ |  | 每股收益(摊薄)(元) | 
 | 11 | diluted_roe | float | 12 |  |  |  | √ |  | 净资产收益率(摊薄)(%) | 
 | 12 | yoy_net_profit | float | 12 |  |  |  | √ |  | 去年同期修正后净利润 | 
 | 13 | is_audit | int |  |  |  |  | √ |  | 是否审计： 1是 0否 | 

## stock_forecast 获取上市公司业绩预告

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | ann_date | date |  |  | √ |  |  |  | 公告日期 | 
 | 2 | ts_code | varchar | 50 |  | √ |  |  |  | TS代码 | 
 | 3 | end_date | date |  |  | √ |  |  |  | 报告期 | 
 | 4 | type | varchar | 255 |  |  |  | √ |  | 业绩预告类型 | 
 | 5 | p_change_min | float | 12 |  |  |  | √ |  | 预告净利润变动幅度下限（%） | 
 | 6 | p_change_max | float | 12 |  |  |  | √ |  | 预告净利润变动幅度上限（%） | 
 | 7 | net_profit_min | float | 12 |  |  |  | √ |  | 预告净利润下限（万元） | 
 | 8 | net_profit_max | float | 12 |  |  |  | √ |  | 预告净利润上限（万元） | 
 | 9 | last_parent_net | float | 12 |  |  |  | √ |  | 上年同期归属母公司净利润 | 
 | 10 | notice_times | int |  |  |  |  | √ |  | 公布次数 | 
 | 11 | first_ann_date | date |  |  |  |  | √ |  | 首次公告日 | 
 | 12 | summary | varchar | 255 |  |  |  | √ |  | 业绩预告摘要 | 
 | 13 | change_reason | text | 65535 |  |  |  | √ |  | 业绩变动原因 | 

## stock_income 获取上市公司财务利润表数据

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | f_ann_date | date |  |  | √ |  |  |  | 实际公告日期 | 
 | 2 | ts_code | varchar | 50 |  | √ |  |  |  | TS代码 | 
 | 3 | ann_date | date |  |  |  |  | √ |  | 公告日期 | 
 | 4 | end_date | date |  |  | √ |  |  |  | 报告期 | 
 | 5 | report_type | float | 12 |  | √ |  |  |  | 报告类型 1合并报表 2单季合并 3调整单季合并表 4调整合并报表 5调整前合并报表 6母公司报表 7母公司单季表 8 母公司调整单季表 9母公司调整表 10母公司调整前报表 11调整前合并报表 12母公司调整前报表 | 
 | 6 | comp_type | float | 12 |  |  |  | √ |  | 公司类型(1一般工商业2银行3保险4证券) | 
 | 7 | basic_eps | float | 12 |  |  |  | √ |  | 基本每股收益 | 
 | 8 | diluted_eps | float | 12 |  |  |  | √ |  | 稀释每股收益 | 
 | 9 | total_revenue | float | 12 |  |  |  | √ |  | 营业总收入 | 
 | 10 | revenue | float | 12 |  |  |  | √ |  | 营业收入 | 
 | 11 | int_income | float | 12 |  |  |  | √ |  | 利息收入 | 
 | 12 | prem_earned | float | 12 |  |  |  | √ |  | 已赚保费 | 
 | 13 | comm_income | float | 12 |  |  |  | √ |  | 手续费及佣金收入 | 
 | 14 | n_commis_income | float | 12 |  |  |  | √ |  | 手续费及佣金净收入 | 
 | 15 | n_oth_income | float | 12 |  |  |  | √ |  | 其他经营净收益 | 
 | 16 | n_oth_b_income | float | 12 |  |  |  | √ |  | 加:其他业务净收益 | 
 | 17 | prem_income | float | 12 |  |  |  | √ |  | 保险业务收入 | 
 | 18 | out_prem | float | 12 |  |  |  | √ |  | 减:分出保费 | 
 | 19 | une_prem_reser | float | 12 |  |  |  | √ |  | 提取未到期责任准备金 | 
 | 20 | reins_income | float | 12 |  |  |  | √ |  | 其中:分保费收入 | 
 | 21 | n_sec_tb_income | float | 12 |  |  |  | √ |  | 代理买卖证券业务净收入 | 
 | 22 | n_sec_uw_income | float | 12 |  |  |  | √ |  | 证券承销业务净收入 | 
 | 23 | n_asset_mg_income | float | 12 |  |  |  | √ |  | 受托客户资产管理业务净收入 | 
 | 24 | oth_b_income | float | 12 |  |  |  | √ |  | 其他业务收入 | 
 | 25 | fv_value_chg_gain | float | 12 |  |  |  | √ |  | 加:公允价值变动净收益 | 
 | 26 | invest_income | float | 12 |  |  |  | √ |  | 加:投资净收益 | 
 | 27 | ass_invest_income | float | 12 |  |  |  | √ |  | 其中:对联营企业和合营企业的投资收益 | 
 | 28 | forex_gain | float | 12 |  |  |  | √ |  | 加:汇兑净收益 | 
 | 29 | total_cogs | float | 12 |  |  |  | √ |  | 营业总成本 | 
 | 30 | oper_cost | float | 12 |  |  |  | √ |  | 减:营业成本 | 
 | 31 | int_exp | float | 12 |  |  |  | √ |  | 减:利息支出 | 
 | 32 | comm_exp | float | 12 |  |  |  | √ |  | 减:手续费及佣金支出 | 
 | 33 | biz_tax_surchg | float | 12 |  |  |  | √ |  | 减:营业税金及附加 | 
 | 34 | sell_exp | float | 12 |  |  |  | √ |  | 减:销售费用 | 
 | 35 | admin_exp | float | 12 |  |  |  | √ |  | 减:管理费用 | 
 | 36 | fin_exp | float | 12 |  |  |  | √ |  | 减:财务费用 | 
 | 37 | assets_impair_loss | float | 12 |  |  |  | √ |  | 减:资产减值损失 | 
 | 38 | prem_refund | float | 12 |  |  |  | √ |  | 退保金 | 
 | 39 | compens_payout | float | 12 |  |  |  | √ |  | 赔付总支出 | 
 | 40 | reser_insur_liab | float | 12 |  |  |  | √ |  | 提取保险责任准备金 | 
 | 41 | div_payt | float | 12 |  |  |  | √ |  | 保户红利支出 | 
 | 42 | reins_exp | float | 12 |  |  |  | √ |  | 分保费用 | 
 | 43 | oper_exp | float | 12 |  |  |  | √ |  | 营业支出 | 
 | 44 | compens_payout_refu | float | 12 |  |  |  | √ |  | 减:摊回赔付支出 | 
 | 45 | insur_reser_refu | float | 12 |  |  |  | √ |  | 减:摊回保险责任准备金 | 
 | 46 | reins_cost_refund | float | 12 |  |  |  | √ |  | 减:摊回分保费用 | 
 | 47 | other_bus_cost | float | 12 |  |  |  | √ |  | 其他业务成本 | 
 | 48 | operate_profit | float | 12 |  |  |  | √ |  | 营业利润 | 
 | 49 | non_oper_income | float | 12 |  |  |  | √ |  | 加:营业外收入 | 
 | 50 | non_oper_exp | float | 12 |  |  |  | √ |  | 减:营业外支出 | 
 | 51 | nca_disploss | float | 12 |  |  |  | √ |  | 其中:减:非流动资产处置净损失 | 
 | 52 | total_profit | float | 12 |  |  |  | √ |  | 利润总额 | 
 | 53 | income_tax | float | 12 |  |  |  | √ |  | 所得税费用 | 
 | 54 | n_income | float | 12 |  |  |  | √ |  | 净利润(含少数股东损益) | 
 | 55 | n_income_attr_p | float | 12 |  |  |  | √ |  | 净利润(不含少数股东损益) | 
 | 56 | minority_gain | float | 12 |  |  |  | √ |  | 少数股东损益 | 
 | 57 | oth_compr_income | float | 12 |  |  |  | √ |  | 其他综合收益 | 
 | 58 | t_compr_income | float | 12 |  |  |  | √ |  | 综合收益总额 | 
 | 59 | compr_inc_attr_p | float | 12 |  |  |  | √ |  | 归属于母公司(或股东)的综合收益总额 | 
 | 60 | compr_inc_attr_m_s | float | 12 |  |  |  | √ |  | 归属于少数股东的综合收益总额 | 
 | 61 | ebit | float | 12 |  |  |  | √ |  | 息税前利润 | 
 | 62 | ebitda | float | 12 |  |  |  | √ |  | 息税折旧摊销前利润 | 
 | 63 | insurance_exp | float | 12 |  |  |  | √ |  | 保险业务支出 | 
 | 64 | undist_profit | float | 12 |  |  |  | √ |  | 年初未分配利润 | 
 | 65 | distable_profit | float | 12 |  |  |  | √ |  | 可分配利润 | 

## trade_cal 获取上证交易所交易日历

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | date | date |  |  | √ |  |  |  | 日期 | 
 | 2 | is_open | tinyint |  | 0 |  |  | √ |  | 是否交易 0休市 1交易 | 
 | 3 | pretrade_date | date |  |  |  |  | √ |  | 上一个交易日 | 


# 2_dwd_index_info


## index_daily_price 指数每日行情

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | code | varchar | 50 |  | √ |  |  |  | 指数代码 | 
 | 2 | date | date |  |  | √ |  |  |  | 日期 | 
 | 3 | open | float | 12 |  |  |  | √ |  | 开盘价 | 
 | 4 | close | float | 12 |  |  |  | √ |  | 收盘价 | 
 | 5 | low | float | 12 |  |  |  | √ |  | 最低价 | 
 | 6 | high | float | 12 |  |  |  | √ |  | 最高价 | 
 | 7 | volume | float | 12 |  |  |  | √ |  | 成交量 | 
 | 8 | money | float | 12 |  |  |  | √ |  | 成交额 | 
 | 9 | vwap | float | 12 |  |  |  | √ |  | 成交量加权均价 | 
 | 10 | pre_close | float | 12 |  |  |  | √ |  | 昨日收盘价 | 
 | 11 | update_time | datetime |  |  |  |  | √ |  | 数据入库时间 | 

## index_info 获取指数基础信息

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | code | varchar | 50 |  | √ |  |  |  | 指数代码 | 
 | 2 | name | varchar | 50 |  |  |  | √ |  | 中文名称 | 
 | 3 | short_name | varchar | 50 |  |  |  | √ |  | 简称 | 
 | 4 | fullname | varchar | 255 |  |  |  | √ |  | 中文全称 | 
 | 5 | market | varchar | 255 |  |  |  | √ |  | 市场 | 
 | 6 | publisher | varchar | 255 |  |  |  | √ |  | 发布方 | 
 | 7 | index_type | varchar | 255 |  |  |  | √ |  | 指数风格 | 
 | 8 | category | varchar | 255 |  |  |  | √ |  | 指数类别 | 
 | 9 | weight_rule | varchar | 255 |  |  |  | √ |  | 加权方式 | 
 | 10 | desc | text | 65535 |  |  |  | √ |  | 描述 | 
 | 11 | base_point | float | 12 |  |  |  | √ |  | 基点 | 
 | 12 | base_date | date |  |  |  |  | √ |  | 基期 | 
 | 13 | publish_date | date |  |  |  |  | √ |  | 发布日期 | 
 | 14 | exp_date | date |  |  |  |  | √ |  | 终止日期 | 
 | 15 | update_time | datetime |  |  |  |  | √ |  | 数据入库时间 | 

## index_jq2ts 聚宽--tushare指数代码映射表

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | jq_code | varchar | 50 |  | √ |  |  |  | 聚宽代码 | 
 | 2 | ts_code | varchar | 50 |  | √ |  |  |  | tushare代码 | 
 | 3 | update_time | datetime |  |  |  |  | √ |  | 数据入库时间 | 

## index_stocks_weights 获取指数成分股及其权重

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | index_code | varchar | 50 |  | √ |  |  |  | 指数代码 | 
 | 2 | date | date |  |  | √ |  |  |  | 更新日期 | 
 | 3 | stock_code | varchar | 50 |  | √ |  |  |  | 股票代码 | 
 | 4 | weight | float | 12 |  |  |  | √ |  | 权重 | 
 | 5 | update_time | datetime |  |  |  |  | √ |  | 数据入库时间 | 


# 2_dwd_industry_info

##industry_all_sw_l1 获取每日申万一级行业列表

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | code | varchar | 50 |  | √ |  |  |  | 行业代码 | 
 | 2 | name | varchar | 50 |  |  |  | √ |  | 行业名称 | 
 | 3 | start_date | date |  |  |  |  | √ |  | 开始日期 | 

## industry_all_sw_l2 获取每日申万二级行业列表

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | code | varchar | 50 |  | √ |  |  |  | 行业代码 | 
 | 2 | name | varchar | 50 |  |  |  | √ |  | 行业名称 | 
 | 3 | start_date | date |  |  |  |  | √ |  | 开始日期 | 

## industry_all_sw_l3 获取每日申万三级行业列表

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | code | varchar | 50 |  | √ |  |  |  | 行业代码 | 
 | 2 | name | varchar | 50 |  |  |  | √ |  | 行业名称 | 
 | 3 | start_date | date |  |  |  |  | √ |  | 开始日期 | 

## industry_stocks_sw_l1 获取申万一级行业成分股

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | date | date |  |  | √ |  |  |  | 日期 | 
 | 2 | industry_code | varchar | 50 |  | √ |  |  |  | 行业代码 | 
 | 3 | stock_code | varchar | 50 |  | √ |  |  |  | 股票代码 | 

## industry_stocks_sw_l2 获取申万二级行业成分股

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | date | date |  |  | √ |  |  |  | 日期 | 
 | 2 | industry_code | varchar | 50 |  | √ |  |  |  | 行业代码 | 
 | 3 | stock_code | varchar | 50 |  | √ |  |  |  | 股票代码 | 

## industry_stocks_sw_l3 获取申万三级行业成分股


# 2_dwd_stock_daily


## days_cal 获取历史日历

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | date | date |  |  | √ |  |  |  | 日期 | 
 | 2 | is_open | tinyint |  | 0 |  |  | √ |  | 是否交易 0休市 1交易 | 
 | 3 | pretrade_date | date |  |  |  |  | √ |  | 上一个交易日 | 
 | 4 | update_time | datetime |  |  |  |  | √ |  | 数据入库时间 | 

## days_trade 获取A股市场交易日历

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | trade_date | date |  |  | √ |  |  |  | 日期 | 
 | 2 | update_time | datetime |  |  |  |  | √ |  | 数据入库时间 | 

## stock_company 获取上市公司基础信息

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | code | varchar | 255 |  | √ |  |  |  | 股票代码 | 
 | 2 | exchange | varchar | 255 |  |  |  | √ |  | 交易所代码SSE上交所 SZSE深交所 | 
 | 3 | chairman | varchar | 255 |  |  |  | √ |  | 法人代表 | 
 | 4 | manager | varchar | 255 |  |  |  | √ |  | 总经理 | 
 | 5 | secretary | varchar | 255 |  |  |  | √ |  | 董秘 | 
 | 6 | reg_capital | float | 12 |  |  |  | √ |  | 注册资本 | 
 | 7 | setup_date | date |  |  |  |  | √ |  | 注册日期 | 
 | 8 | province | varchar | 255 |  |  |  | √ |  | 所在省份 | 
 | 9 | city | varchar | 255 |  |  |  | √ |  | 所在城市 | 
 | 10 | introduction | text | 65535 |  |  |  | √ |  | 公司介绍 | 
 | 11 | website | varchar | 255 |  |  |  | √ |  | 公司主页 | 
 | 12 | email | varchar | 255 |  |  |  | √ |  | 电子邮件 | 
 | 13 | office | varchar | 255 |  |  |  | √ |  | 办公室 | 
 | 14 | ann_date | date |  |  |  |  | √ |  | 公告日期 | 
 | 15 | business_scope | text | 65535 |  |  |  | √ |  | 经营范围 | 
 | 16 | employees | int |  |  |  |  | √ |  | 员工人数 | 
 | 17 | main_business | text | 65535 |  |  |  | √ |  | 主要业务及产品 | 

## stock_daily_indicator 股票每日市值相关指标

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | code | varchar | 50 |  | √ |  |  |  | 股票代码 | 
 | 2 | date | date |  |  | √ |  |  |  | 日期 | 
 | 3 | capitalization | float | 12 |  |  |  | √ |  | 总股本(万股) | 
 | 4 | circulating_cap | float | 12 |  |  |  | √ |  | 流通股本(万股) | 
 | 5 | market_cap | float | 12 |  |  |  | √ |  | 总市值(亿元) | 
 | 6 | circulating_market_cap | float | 12 |  |  |  | √ |  | 流通市值(亿元) | 
 | 7 | turnover_ratio | float | 12 |  |  |  | √ |  | 换手率(%) | 
 | 8 | pe_ratio | float | 12 |  |  |  | √ |  | 市盈率(PE, TTM) | 
 | 9 | pe_ratio_lyr | float | 12 |  |  |  | √ |  | 市盈率(PE) | 
 | 10 | pb_ratio | float | 12 |  |  |  | √ |  | 市净率(PB) | 
 | 11 | ps_ratio | float | 12 |  |  |  | √ |  | 市销率(PS, TTM) | 
 | 12 | pcf_ratio | float | 12 |  |  |  | √ |  | 市现率(PCF, 现金净流量TTM) | 
 | 13 | update_time | datetime |  |  |  |  | √ |  | 数据入库时间 | 

## stock_daily_industry 股票每日所属行业详情

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | code | varchar | 50 |  | √ |  |  |  | 股票代码 | 
 | 2 | date | date |  |  | √ |  |  |  | 日期 | 
 | 3 | jq_l1 | varchar | 50 |  |  |  | √ |  | 聚宽一级行业 | 
 | 4 | jq_l2 | varchar | 50 |  |  |  | √ |  | 聚宽二级行业 | 
 | 5 | sw_l1 | varchar | 50 |  |  |  | √ |  | 申万一级行业 | 
 | 6 | sw_l2 | varchar | 50 |  |  |  | √ |  | 申万二级行业 | 
 | 7 | sw_l3 | varchar | 50 |  |  |  | √ |  | 申万三级行业 | 
 | 8 | zjw | varchar | 50 |  |  |  | √ |  | 证监会行业 | 
 | 9 | update_time | datetime |  |  |  |  | √ |  | 数据入库时间 | 

## stock_daily_price 股票每日行情--价格不复权

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | code | varchar | 50 |  | √ |  |  |  | 股票代码 | 
 | 2 | date | date |  |  | √ |  |  |  | 日期 | 
 | 3 | open | float | 12 |  |  |  | √ |  | 开盘价 | 
 | 4 | close | float | 12 |  |  |  | √ |  | 收盘价 | 
 | 5 | low | float | 12 |  |  |  | √ |  | 最低价 | 
 | 6 | high | float | 12 |  |  |  | √ |  | 最高价 | 
 | 7 | volume | float | 12 |  |  |  | √ |  | 成交量 | 
 | 8 | money | float | 12 |  |  |  | √ |  | 成交额 | 
 | 9 | factor | float | 12 |  |  |  | √ |  | 复权因子 | 
 | 10 | high_limit | float | 12 |  |  |  | √ |  | 涨停价 | 
 | 11 | low_limit | float | 12 |  |  |  | √ |  | 跌停价 | 
 | 12 | vwap | float | 12 |  |  |  | √ |  | 成交量加权均价 | 
 | 13 | pre_close | float | 12 |  |  |  | √ |  | 昨日收盘价 | 
 | 14 | paused | tinyint |  | 0 |  |  | √ |  | 是否停牌 | 
 | 15 | is_st | tinyint |  | 0 |  |  | √ |  | 是否st,*st和退市整理期标的 | 
 | 16 | update_time | datetime |  |  |  |  | √ |  | 数据入库时间 | 

## stock_daily_price_post 股票每日行情--价格后复权

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | code | varchar | 50 |  | √ |  |  |  | 股票代码 | 
 | 2 | date | date |  |  | √ |  |  |  | 日期 | 
 | 3 | open | float | 12 |  |  |  | √ |  | 开盘价 | 
 | 4 | close | float | 12 |  |  |  | √ |  | 收盘价 | 
 | 5 | low | float | 12 |  |  |  | √ |  | 最低价 | 
 | 6 | high | float | 12 |  |  |  | √ |  | 最高价 | 
 | 7 | volume | float | 12 |  |  |  | √ |  | 成交量 | 
 | 8 | money | float | 12 |  |  |  | √ |  | 成交额 | 
 | 9 | factor | float | 12 |  |  |  | √ |  | 复权因子 | 
 | 10 | high_limit | float | 12 |  |  |  | √ |  | 涨停价 | 
 | 11 | low_limit | float | 12 |  |  |  | √ |  | 跌停价 | 
 | 12 | vwap | float | 12 |  |  |  | √ |  | 成交量加权均价 | 
 | 13 | pre_close | float | 12 |  |  |  | √ |  | 昨日收盘价 | 
 | 14 | paused | tinyint |  | 0 |  |  | √ |  | 是否停牌 | 
 | 15 | is_st | tinyint |  | 0 |  |  | √ |  | 是否st,*st和退市整理期标的 | 
 | 16 | update_time | datetime |  |  |  |  | √ |  | 数据入库时间 | 

## stock_info 获取 A 股市场全体股票及其简要概况

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | code | varchar | 50 |  | √ |  |  |  | 股票代码 | 
 | 2 | display_name | varchar | 50 |  |  |  | √ |  | 中文名称 | 
 | 3 | name | varchar | 50 |  |  |  | √ |  | 简称 | 
 | 4 | start_date | date |  |  |  |  | √ |  | 上市日期 | 
 | 5 | end_date | date |  |  |  |  | √ |  | 退市日期，如果没有退市则为2200-01-01 | 
 | 6 | type | varchar | 50 |  |  |  | √ |  | 类型 | 

# 2_dwd_stock_finance

## stock_dividend 获取上市公司分红送股数据

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | code | varchar | 50 |  | √ |  |  |  | 股票代码 | 
 | 2 | date | date |  |  | √ |  |  |  | 预案公告日（董事会） | 
 | 3 | end_date | date |  |  | √ |  |  |  | 分送年度 | 
 | 4 | div_proc | varchar | 255 |  | √ |  |  |  | 实施进度 | 
 | 5 | stk_div | float | 12 |  |  |  | √ |  | 每股送转 | 
 | 6 | stk_bo_rate | float | 12 |  |  |  | √ |  | 每股送股比例 | 
 | 7 | stk_co_rate | float | 12 |  |  |  | √ |  | 每股转增比例 | 
 | 8 | cash_div | float | 12 |  |  |  | √ |  | 每股分红（税后） | 
 | 9 | cash_div_tax | float | 12 |  |  |  | √ |  | 每股分红（税前） | 
 | 10 | record_date | date |  |  |  |  | √ |  | 股权登记日 | 
 | 11 | ex_date | date |  |  |  |  | √ |  | 除权除息日 | 
 | 12 | pay_date | date |  |  |  |  | √ |  | 派息日 | 
 | 13 | div_listdate | date |  |  |  |  | √ |  | 红股上市日 | 
 | 14 | imp_ann_date | date |  |  |  |  | √ |  | 实施公告日 | 
 | 15 | base_date | date |  |  |  |  | √ |  | 基准日 | 
 | 16 | base_share | float | 12 |  |  |  | √ |  | 实施基准股本（万） | 
 | 17 | update_flag | float | 12 |  |  |  | √ |  | 是否变更过（1表示变更） | 

## stock_express 获取上市公司业绩快报

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | code | varchar | 50 |  | √ |  |  |  | 股票代码 | 
 | 2 | date | date |  |  | √ |  |  |  | 公告日期 | 
 | 3 | end_date | date |  |  | √ |  |  |  | 报告期 | 
 | 4 | revenue | float | 12 |  |  |  | √ |  | 营业收入(元) | 
 | 5 | operate_profit | float | 12 |  |  |  | √ |  | 营业利润(元) | 
 | 6 | total_profit | float | 12 |  |  |  | √ |  | 利润总额(元) | 
 | 7 | n_income | float | 12 |  |  |  | √ |  | 净利润(元) | 
 | 8 | total_assets | float | 12 |  |  |  | √ |  | 总资产(元) | 
 | 9 | total_hldr_eqy_exc_min_int | float | 12 |  |  |  | √ |  | 股东权益合计(不含少数股东权益)(元) | 
 | 10 | diluted_eps | float | 12 |  |  |  | √ |  | 每股收益(摊薄)(元) | 
 | 11 | diluted_roe | float | 12 |  |  |  | √ |  | 净资产收益率(摊薄)(%) | 
 | 12 | yoy_net_profit | float | 12 |  |  |  | √ |  | 去年同期修正后净利润 | 
 | 13 | is_audit | int |  |  |  |  | √ |  | 是否审计： 1是 0否 | 

## stock_forecast 获取上市公司业绩预告

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | code | varchar | 50 |  | √ |  |  |  | 股票代码 | 
 | 2 | date | date |  |  | √ |  |  |  | 公告日期 | 
 | 3 | end_date | date |  |  | √ |  |  |  | 报告期 | 
 | 4 | type | varchar | 255 |  |  |  | √ |  | 业绩预告类型 | 
 | 5 | p_change_min | float | 12 |  |  |  | √ |  | 预告净利润变动幅度下限（%） | 
 | 6 | p_change_max | float | 12 |  |  |  | √ |  | 预告净利润变动幅度上限（%） | 
 | 7 | net_profit_min | float | 12 |  |  |  | √ |  | 预告净利润下限（万元） | 
 | 8 | net_profit_max | float | 12 |  |  |  | √ |  | 预告净利润上限（万元） | 
 | 9 | last_parent_net | float | 12 |  |  |  | √ |  | 上年同期归属母公司净利润 | 
 | 10 | notice_times | int |  |  |  |  | √ |  | 公布次数 | 
 | 11 | first_ann_date | date |  |  |  |  | √ |  | 首次公告日 | 
 | 12 | summary | varchar | 255 |  |  |  | √ |  | 业绩预告摘要 | 
 | 13 | change_reason | text | 65535 |  |  |  | √ |  | 业绩变动原因 | 

## stock_report_balance 获取上市公司报告期资产负债表

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | code | varchar | 50 |  | √ |  |  |  | 股票代码 | 
 | 2 | date | date |  |  | √ |  |  |  | 公告日期 | 
 | 3 | ann_date | date |  |  |  |  | √ |  | 最初公告日期（便于查找数据修改前的版本） | 
 | 4 | end_date | date |  |  | √ |  |  |  | 报告期 | 
 | 5 | report_type | float | 12 |  | √ |  |  |  | 报告类型 1合并报表 2单季合并 3调整单季合并表 4调整合并报表 5调整前合并报表 6母公司报表 7母公司单季表 8 母公司调整单季表 9母公司调整表 10母公司调整前报表 11调整前合并报表 12母公司调整前报表 | 
 | 6 | comp_type | float | 12 |  |  |  | √ |  | 公司类型(1一般工商业2银行3保险4证券) | 
 | 7 | total_share | float | 12 |  |  |  | √ |  | 期末总股本 | 
 | 8 | cap_rese | float | 12 |  |  |  | √ |  | 资本公积金 | 
 | 9 | undistr_porfit | float | 12 |  |  |  | √ |  | 未分配利润 | 
 | 10 | surplus_rese | float | 12 |  |  |  | √ |  | 盈余公积金 | 
 | 11 | special_rese | float | 12 |  |  |  | √ |  | 专项储备 | 
 | 12 | money_cap | float | 12 |  |  |  | √ |  | 货币资金 | 
 | 13 | trad_asset | float | 12 |  |  |  | √ |  | 交易性金融资产 | 
 | 14 | notes_receiv | float | 12 |  |  |  | √ |  | 应收票据 | 
 | 15 | accounts_receiv | float | 12 |  |  |  | √ |  | 应收账款 | 
 | 16 | oth_receiv | float | 12 |  |  |  | √ |  | 其他应收款 | 
 | 17 | prepayment | float | 12 |  |  |  | √ |  | 预付款项 | 
 | 18 | div_receiv | float | 12 |  |  |  | √ |  | 应收股利 | 
 | 19 | int_receiv | float | 12 |  |  |  | √ |  | 应收利息 | 
 | 20 | inventories | float | 12 |  |  |  | √ |  | 存货 | 
 | 21 | amor_exp | float | 12 |  |  |  | √ |  | 长期待摊费用 | 
 | 22 | nca_within_1y | float | 12 |  |  |  | √ |  | 一年内到期的非流动资产 | 
 | 23 | sett_rsrv | float | 12 |  |  |  | √ |  | 结算备付金 | 
 | 24 | loanto_oth_bank_fi | float | 12 |  |  |  | √ |  | 拆出资金 | 
 | 25 | premium_receiv | float | 12 |  |  |  | √ |  | 应收保费 | 
 | 26 | reinsur_receiv | float | 12 |  |  |  | √ |  | 应收分保账款 | 
 | 27 | reinsur_res_receiv | float | 12 |  |  |  | √ |  | 应收分保合同准备金 | 
 | 28 | pur_resale_fa | float | 12 |  |  |  | √ |  | 买入返售金融资产 | 
 | 29 | oth_cur_assets | float | 12 |  |  |  | √ |  | 其他流动资产 | 
 | 30 | total_cur_assets | float | 12 |  |  |  | √ |  | 流动资产合计 | 
 | 31 | fa_avail_for_sale | float | 12 |  |  |  | √ |  | 可供出售金融资产 | 
 | 32 | htm_invest | float | 12 |  |  |  | √ |  | 持有至到期投资 | 
 | 33 | lt_eqt_invest | float | 12 |  |  |  | √ |  | 长期股权投资 | 
 | 34 | invest_real_estate | float | 12 |  |  |  | √ |  | 投资性房地产 | 
 | 35 | time_deposits | float | 12 |  |  |  | √ |  | 定期存款 | 
 | 36 | oth_assets | float | 12 |  |  |  | √ |  | 其他资产 | 
 | 37 | lt_rec | float | 12 |  |  |  | √ |  | 长期应收款 | 
 | 38 | fix_assets | float | 12 |  |  |  | √ |  | 固定资产 | 
 | 39 | cip | float | 12 |  |  |  | √ |  | 在建工程 | 
 | 40 | const_materials | float | 12 |  |  |  | √ |  | 工程物资 | 
 | 41 | fixed_assets_disp | float | 12 |  |  |  | √ |  | 固定资产清理 | 
 | 42 | produc_bio_assets | float | 12 |  |  |  | √ |  | 生产性生物资产 | 
 | 43 | oil_and_gas_assets | float | 12 |  |  |  | √ |  | 油气资产 | 
 | 44 | intan_assets | float | 12 |  |  |  | √ |  | 无形资产 | 
 | 45 | r_and_d | float | 12 |  |  |  | √ |  | 研发支出 | 
 | 46 | goodwill | float | 12 |  |  |  | √ |  | 商誉 | 
 | 47 | lt_amor_exp | float | 12 |  |  |  | √ |  | 长期待摊费用 | 
 | 48 | defer_tax_assets | float | 12 |  |  |  | √ |  | 递延所得税资产 | 
 | 49 | decr_in_disbur | float | 12 |  |  |  | √ |  | 发放贷款及垫款 | 
 | 50 | oth_nca | float | 12 |  |  |  | √ |  | 其他非流动资产 | 
 | 51 | total_nca | float | 12 |  |  |  | √ |  | 非流动资产合计 | 
 | 52 | cash_reser_cb | float | 12 |  |  |  | √ |  | 现金及存放中央银行款项 | 
 | 53 | depos_in_oth_bfi | float | 12 |  |  |  | √ |  | 存放同业和其它金融机构款项 | 
 | 54 | prec_metals | float | 12 |  |  |  | √ |  | 贵金属 | 
 | 55 | deriv_assets | float | 12 |  |  |  | √ |  | 衍生金融资产 | 
 | 56 | rr_reins_une_prem | float | 12 |  |  |  | √ |  | 应收分保未到期责任准备金 | 
 | 57 | rr_reins_outstd_cla | float | 12 |  |  |  | √ |  | 应收分保未决赔款准备金 | 
 | 58 | rr_reins_lins_liab | float | 12 |  |  |  | √ |  | 应收分保寿险责任准备金 | 
 | 59 | rr_reins_lthins_liab | float | 12 |  |  |  | √ |  | 应收分保长期健康险责任准备金 | 
 | 60 | refund_depos | float | 12 |  |  |  | √ |  | 存出保证金 | 
 | 61 | ph_pledge_loans | float | 12 |  |  |  | √ |  | 保户质押贷款 | 
 | 62 | refund_cap_depos | float | 12 |  |  |  | √ |  | 存出资本保证金 | 
 | 63 | indep_acct_assets | float | 12 |  |  |  | √ |  | 独立账户资产 | 
 | 64 | client_depos | float | 12 |  |  |  | √ |  | 其中：客户资金存款 | 
 | 65 | client_prov | float | 12 |  |  |  | √ |  | 其中：客户备付金 | 
 | 66 | transac_seat_fee | float | 12 |  |  |  | √ |  | 其中:交易席位费 | 
 | 67 | invest_as_receiv | float | 12 |  |  |  | √ |  | 应收款项类投资 | 
 | 68 | total_assets | float | 12 |  |  |  | √ |  | 资产总计 | 
 | 69 | lt_borr | float | 12 |  |  |  | √ |  | 长期借款 | 
 | 70 | st_borr | float | 12 |  |  |  | √ |  | 短期借款 | 
 | 71 | cb_borr | float | 12 |  |  |  | √ |  | 向中央银行借款 | 
 | 72 | depos_ib_deposits | float | 12 |  |  |  | √ |  | 吸收存款及同业存放 | 
 | 73 | loan_oth_bank | float | 12 |  |  |  | √ |  | 拆入资金 | 
 | 74 | trading_fl | float | 12 |  |  |  | √ |  | 交易性金融负债 | 
 | 75 | notes_payable | float | 12 |  |  |  | √ |  | 应付票据 | 
 | 76 | acct_payable | float | 12 |  |  |  | √ |  | 应付账款 | 
 | 77 | adv_receipts | float | 12 |  |  |  | √ |  | 预收款项 | 
 | 78 | sold_for_repur_fa | float | 12 |  |  |  | √ |  | 卖出回购金融资产款 | 
 | 79 | comm_payable | float | 12 |  |  |  | √ |  | 应付手续费及佣金 | 
 | 80 | payroll_payable | float | 12 |  |  |  | √ |  | 应付职工薪酬 | 
 | 81 | taxes_payable | float | 12 |  |  |  | √ |  | 应交税费 | 
 | 82 | int_payable | float | 12 |  |  |  | √ |  | 应付利息 | 
 | 83 | div_payable | float | 12 |  |  |  | √ |  | 应付股利 | 
 | 84 | oth_payable | float | 12 |  |  |  | √ |  | 其他应付款 | 
 | 85 | acc_exp | float | 12 |  |  |  | √ |  | 预提费用 | 
 | 86 | deferred_inc | float | 12 |  |  |  | √ |  | 递延收益 | 
 | 87 | st_bonds_payable | float | 12 |  |  |  | √ |  | 应付短期债券 | 
 | 88 | payable_to_reinsurer | float | 12 |  |  |  | √ |  | 应付分保账款 | 
 | 89 | rsrv_insur_cont | float | 12 |  |  |  | √ |  | 保险合同准备金 | 
 | 90 | acting_trading_sec | float | 12 |  |  |  | √ |  | 代理买卖证券款 | 
 | 91 | acting_uw_sec | float | 12 |  |  |  | √ |  | 代理承销证券款 | 
 | 92 | non_cur_liab_due_1y | float | 12 |  |  |  | √ |  | 一年内到期的非流动负债 | 
 | 93 | oth_cur_liab | float | 12 |  |  |  | √ |  | 其他流动负债 | 
 | 94 | total_cur_liab | float | 12 |  |  |  | √ |  | 流动负债合计 | 
 | 95 | bond_payable | float | 12 |  |  |  | √ |  | 应付债券 | 
 | 96 | lt_payable | float | 12 |  |  |  | √ |  | 长期应付款 | 
 | 97 | specific_payables | float | 12 |  |  |  | √ |  | 专项应付款 | 
 | 98 | estimated_liab | float | 12 |  |  |  | √ |  | 预计负债 | 
 | 99 | defer_tax_liab | float | 12 |  |  |  | √ |  | 递延所得税负债 | 
 | 100 | defer_inc_non_cur_liab | float | 12 |  |  |  | √ |  | 递延收益-非流动负债 | 
 | 101 | oth_ncl | float | 12 |  |  |  | √ |  | 其他非流动负债 | 
 | 102 | total_ncl | float | 12 |  |  |  | √ |  | 非流动负债合计 | 
 | 103 | depos_oth_bfi | float | 12 |  |  |  | √ |  | 同业和其它金融机构存放款项 | 
 | 104 | deriv_liab | float | 12 |  |  |  | √ |  | 衍生金融负债 | 
 | 105 | depos | float | 12 |  |  |  | √ |  | 吸收存款 | 
 | 106 | agency_bus_liab | float | 12 |  |  |  | √ |  | 代理业务负债 | 
 | 107 | oth_liab | float | 12 |  |  |  | √ |  | 其他负债 | 
 | 108 | prem_receiv_adva | float | 12 |  |  |  | √ |  | 预收保费 | 
 | 109 | depos_received | float | 12 |  |  |  | √ |  | 存入保证金 | 
 | 110 | ph_invest | float | 12 |  |  |  | √ |  | 保户储金及投资款 | 
 | 111 | reser_une_prem | float | 12 |  |  |  | √ |  | 未到期责任准备金 | 
 | 112 | reser_outstd_claims | float | 12 |  |  |  | √ |  | 未决赔款准备金 | 
 | 113 | reser_lins_liab | float | 12 |  |  |  | √ |  | 寿险责任准备金 | 
 | 114 | reser_lthins_liab | float | 12 |  |  |  | √ |  | 长期健康险责任准备金 | 
 | 115 | indept_acc_liab | float | 12 |  |  |  | √ |  | 独立账户负债 | 
 | 116 | pledge_borr | float | 12 |  |  |  | √ |  | 其中:质押借款 | 
 | 117 | indem_payable | float | 12 |  |  |  | √ |  | 应付赔付款 | 
 | 118 | policy_div_payable | float | 12 |  |  |  | √ |  | 应付保单红利 | 
 | 119 | total_liab | float | 12 |  |  |  | √ |  | 负债合计 | 
 | 120 | treasury_share | float | 12 |  |  |  | √ |  | 减:库存股 | 
 | 121 | ordin_risk_reser | float | 12 |  |  |  | √ |  | 一般风险准备 | 
 | 122 | forex_differ | float | 12 |  |  |  | √ |  | 外币报表折算差额 | 
 | 123 | invest_loss_unconf | float | 12 |  |  |  | √ |  | 未确认的投资损失 | 
 | 124 | minority_int | float | 12 |  |  |  | √ |  | 少数股东权益 | 
 | 125 | total_hldr_eqy_exc_min_int | float | 12 |  |  |  | √ |  | 股东权益合计(不含少数股东权益) | 
 | 126 | total_hldr_eqy_inc_min_int | float | 12 |  |  |  | √ |  | 股东权益合计(含少数股东权益) | 
 | 127 | total_liab_hldr_eqy | float | 12 |  |  |  | √ |  | 负债及股东权益总计 | 
 | 128 | lt_payroll_payable | float | 12 |  |  |  | √ |  | 长期应付职工薪酬 | 
 | 129 | oth_comp_income | float | 12 |  |  |  | √ |  | 其他综合收益 | 
 | 130 | oth_eqt_tools | float | 12 |  |  |  | √ |  | 其他权益工具 | 
 | 131 | oth_eqt_tools_p_shr | float | 12 |  |  |  | √ |  | 其他权益工具(优先股) | 
 | 132 | lending_funds | float | 12 |  |  |  | √ |  | 融出资金 | 
 | 133 | acc_receivable | float | 12 |  |  |  | √ |  | 应收款项 | 
 | 134 | st_fin_payable | float | 12 |  |  |  | √ |  | 应付短期融资款 | 
 | 135 | payables | float | 12 |  |  |  | √ |  | 应付款项 | 
 | 136 | hfs_assets | float | 12 |  |  |  | √ |  | 持有待售的资产 | 
 | 137 | hfs_sales | float | 12 |  |  |  | √ |  | 持有待售的负债 | 
 | 138 | update_time | datetime |  |  |  |  | √ |  | 数据入库时间 | 

## stock_report_cashflow 获取上市公司报告期现金流量表

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | code | varchar | 50 |  | √ |  |  |  | 股票代码 | 
 | 2 | date | date |  |  | √ |  |  |  | 公告日期 | 
 | 3 | ann_date | date |  |  |  |  | √ |  | 最初公告日期（便于查找数据修改前的版本） | 
 | 4 | end_date | date |  |  | √ |  |  |  | 报告期 | 
 | 5 | report_type | float | 12 |  | √ |  |  |  | 报告类型 1合并报表 2单季合并 3调整单季合并表 4调整合并报表 5调整前合并报表 6母公司报表 7母公司单季表 8 母公司调整单季表 9母公司调整表 10母公司调整前报表 11调整前合并报表 12母公司调整前报表 | 
 | 6 | comp_type | float | 12 |  |  |  | √ |  | 公司类型(1一般工商业2银行3保险4证券) | 
 | 7 | net_profit | float | 12 |  |  |  | √ |  | 净利润 | 
 | 8 | finan_exp | float | 12 |  |  |  | √ |  | 财务费用 | 
 | 9 | c_fr_sale_sg | float | 12 |  |  |  | √ |  | 销售商品、提供劳务收到的现金 | 
 | 10 | recp_tax_rends | float | 12 |  |  |  | √ |  | 收到的税费返还 | 
 | 11 | n_depos_incr_fi | float | 12 |  |  |  | √ |  | 客户存款和同业存放款项净增加额 | 
 | 12 | n_incr_loans_cb | float | 12 |  |  |  | √ |  | 向中央银行借款净增加额 | 
 | 13 | n_inc_borr_oth_fi | float | 12 |  |  |  | √ |  | 向其他金融机构拆入资金净增加额 | 
 | 14 | prem_fr_orig_contr | float | 12 |  |  |  | √ |  | 收到原保险合同保费取得的现金 | 
 | 15 | n_incr_insured_dep | float | 12 |  |  |  | √ |  | 保户储金净增加额 | 
 | 16 | n_reinsur_prem | float | 12 |  |  |  | √ |  | 收到再保业务现金净额 | 
 | 17 | n_incr_disp_tfa | float | 12 |  |  |  | √ |  | 处置交易性金融资产净增加额 | 
 | 18 | ifc_cash_incr | float | 12 |  |  |  | √ |  | 收取利息和手续费净增加额 | 
 | 19 | n_incr_disp_faas | float | 12 |  |  |  | √ |  | 处置可供出售金融资产净增加额 | 
 | 20 | n_incr_loans_oth_bank | float | 12 |  |  |  | √ |  | 拆入资金净增加额 | 
 | 21 | n_cap_incr_repur | float | 12 |  |  |  | √ |  | 回购业务资金净增加额 | 
 | 22 | c_fr_oth_operate_a | float | 12 |  |  |  | √ |  | 收到其他与经营活动有关的现金 | 
 | 23 | c_inf_fr_operate_a | float | 12 |  |  |  | √ |  | 经营活动现金流入小计 | 
 | 24 | c_paid_goods_s | float | 12 |  |  |  | √ |  | 购买商品、接受劳务支付的现金 | 
 | 25 | c_paid_to_for_empl | float | 12 |  |  |  | √ |  | 支付给职工以及为职工支付的现金 | 
 | 26 | c_paid_for_taxes | float | 12 |  |  |  | √ |  | 支付的各项税费 | 
 | 27 | n_incr_clt_loan_adv | float | 12 |  |  |  | √ |  | 客户贷款及垫款净增加额 | 
 | 28 | n_incr_dep_cbob | float | 12 |  |  |  | √ |  | 存放央行和同业款项净增加额 | 
 | 29 | c_pay_claims_orig_inco | float | 12 |  |  |  | √ |  | 支付原保险合同赔付款项的现金 | 
 | 30 | pay_handling_chrg | float | 12 |  |  |  | √ |  | 支付手续费的现金 | 
 | 31 | pay_comm_insur_plcy | float | 12 |  |  |  | √ |  | 支付保单红利的现金 | 
 | 32 | oth_cash_pay_oper_act | float | 12 |  |  |  | √ |  | 支付其他与经营活动有关的现金 | 
 | 33 | st_cash_out_act | float | 12 |  |  |  | √ |  | 经营活动现金流出小计 | 
 | 34 | n_cashflow_act | float | 12 |  |  |  | √ |  | 经营活动产生的现金流量净额 | 
 | 35 | oth_recp_ral_inv_act | float | 12 |  |  |  | √ |  | 收到其他与投资活动有关的现金 | 
 | 36 | c_disp_withdrwl_invest | float | 12 |  |  |  | √ |  | 收回投资收到的现金 | 
 | 37 | c_recp_return_invest | float | 12 |  |  |  | √ |  | 取得投资收益收到的现金 | 
 | 38 | n_recp_disp_fiolta | float | 12 |  |  |  | √ |  | 处置固定资产、无形资产和其他长期资产收回的现金净额 | 
 | 39 | n_recp_disp_sobu | float | 12 |  |  |  | √ |  | 处置子公司及其他营业单位收到的现金净额 | 
 | 40 | stot_inflows_inv_act | float | 12 |  |  |  | √ |  | 投资活动现金流入小计 | 
 | 41 | c_pay_acq_const_fiolta | float | 12 |  |  |  | √ |  | 购建固定资产、无形资产和其他长期资产支付的现金 | 
 | 42 | c_paid_invest | float | 12 |  |  |  | √ |  | 投资支付的现金 | 
 | 43 | n_disp_subs_oth_biz | float | 12 |  |  |  | √ |  | 取得子公司及其他营业单位支付的现金净额 | 
 | 44 | oth_pay_ral_inv_act | float | 12 |  |  |  | √ |  | 支付其他与投资活动有关的现金 | 
 | 45 | n_incr_pledge_loan | float | 12 |  |  |  | √ |  | 质押贷款净增加额 | 
 | 46 | stot_out_inv_act | float | 12 |  |  |  | √ |  | 投资活动现金流出小计 | 
 | 47 | n_cashflow_inv_act | float | 12 |  |  |  | √ |  | 投资活动产生的现金流量净额 | 
 | 48 | c_recp_borrow | float | 12 |  |  |  | √ |  | 取得借款收到的现金 | 
 | 49 | proc_issue_bonds | float | 12 |  |  |  | √ |  | 发行债券收到的现金 | 
 | 50 | oth_cash_recp_ral_fnc_act | float | 12 |  |  |  | √ |  | 收到其他与筹资活动有关的现金 | 
 | 51 | stot_cash_in_fnc_act | float | 12 |  |  |  | √ |  | 筹资活动现金流入小计 | 
 | 52 | free_cashflow | float | 12 |  |  |  | √ |  | 企业自由现金流量 | 
 | 53 | c_prepay_amt_borr | float | 12 |  |  |  | √ |  | 偿还债务支付的现金 | 
 | 54 | c_pay_dist_dpcp_int_exp | float | 12 |  |  |  | √ |  | 分配股利、利润或偿付利息支付的现金 | 
 | 55 | incl_dvd_profit_paid_sc_ms | float | 12 |  |  |  | √ |  | 其中:子公司支付给少数股东的股利、利润 | 
 | 56 | oth_cashpay_ral_fnc_act | float | 12 |  |  |  | √ |  | 支付其他与筹资活动有关的现金 | 
 | 57 | stot_cashout_fnc_act | float | 12 |  |  |  | √ |  | 筹资活动现金流出小计 | 
 | 58 | n_cash_flows_fnc_act | float | 12 |  |  |  | √ |  | 筹资活动产生的现金流量净额 | 
 | 59 | eff_fx_flu_cash | float | 12 |  |  |  | √ |  | 汇率变动对现金的影响 | 
 | 60 | n_incr_cash_cash_equ | float | 12 |  |  |  | √ |  | 现金及现金等价物净增加额 | 
 | 61 | c_cash_equ_beg_period | float | 12 |  |  |  | √ |  | 期初现金及现金等价物余额 | 
 | 62 | c_cash_equ_end_period | float | 12 |  |  |  | √ |  | 期末现金及现金等价物余额 | 
 | 63 | c_recp_cap_contrib | float | 12 |  |  |  | √ |  | 吸收投资收到的现金 | 
 | 64 | incl_cash_rec_saims | float | 12 |  |  |  | √ |  | 其中:子公司吸收少数股东投资收到的现金 | 
 | 65 | uncon_invest_loss | float | 12 |  |  |  | √ |  | 未确认投资损失 | 
 | 66 | prov_depr_assets | float | 12 |  |  |  | √ |  | 加:资产减值准备 | 
 | 67 | depr_fa_coga_dpba | float | 12 |  |  |  | √ |  | 固定资产折旧、油气资产折耗、生产性生物资产折旧 | 
 | 68 | amort_intang_assets | float | 12 |  |  |  | √ |  | 无形资产摊销 | 
 | 69 | lt_amort_deferred_exp | float | 12 |  |  |  | √ |  | 长期待摊费用摊销 | 
 | 70 | decr_deferred_exp | float | 12 |  |  |  | √ |  | 待摊费用减少 | 
 | 71 | incr_acc_exp | float | 12 |  |  |  | √ |  | 预提费用增加 | 
 | 72 | loss_disp_fiolta | float | 12 |  |  |  | √ |  | 处置固定、无形资产和其他长期资产的损失 | 
 | 73 | loss_scr_fa | float | 12 |  |  |  | √ |  | 固定资产报废损失 | 
 | 74 | loss_fv_chg | float | 12 |  |  |  | √ |  | 公允价值变动损失 | 
 | 75 | invest_loss | float | 12 |  |  |  | √ |  | 投资损失 | 
 | 76 | decr_def_inc_tax_assets | float | 12 |  |  |  | √ |  | 递延所得税资产减少 | 
 | 77 | incr_def_inc_tax_liab | float | 12 |  |  |  | √ |  | 递延所得税负债增加 | 
 | 78 | decr_inventories | float | 12 |  |  |  | √ |  | 存货的减少 | 
 | 79 | decr_oper_payable | float | 12 |  |  |  | √ |  | 经营性应收项目的减少 | 
 | 80 | incr_oper_payable | float | 12 |  |  |  | √ |  | 经营性应付项目的增加 | 
 | 81 | others | float | 12 |  |  |  | √ |  | 其他 | 
 | 82 | im_net_cashflow_oper_act | float | 12 |  |  |  | √ |  | 经营活动产生的现金流量净额(间接法) | 
 | 83 | conv_debt_into_cap | float | 12 |  |  |  | √ |  | 债务转为资本 | 
 | 84 | conv_copbonds_due_within_1y | float | 12 |  |  |  | √ |  | 一年内到期的可转换公司债券 | 
 | 85 | fa_fnc_leases | float | 12 |  |  |  | √ |  | 融资租入固定资产 | 
 | 86 | end_bal_cash | float | 12 |  |  |  | √ |  | 现金的期末余额 | 
 | 87 | beg_bal_cash | float | 12 |  |  |  | √ |  | 减:现金的期初余额 | 
 | 88 | end_bal_cash_equ | float | 12 |  |  |  | √ |  | 加:现金等价物的期末余额 | 
 | 89 | beg_bal_cash_equ | float | 12 |  |  |  | √ |  | 减:现金等价物的期初余额 | 
 | 90 | im_n_incr_cash_equ | float | 12 |  |  |  | √ |  | 现金及现金等价物净增加额(间接法) | 
 | 91 | update_time | datetime |  |  |  |  | √ |  | 数据入库时间 | 

## stock_report_income 获取上市公司报告期财务利润表数据

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | code | varchar | 50 |  | √ |  |  |  | 股票代码 | 
 | 2 | date | date |  |  | √ |  |  |  | 公告日期 | 
 | 3 | ann_date | date |  |  |  |  | √ |  | 最初公告日期（便于查找数据修改前的版本） | 
 | 4 | end_date | date |  |  | √ |  |  |  | 报告期 | 
 | 5 | report_type | float | 12 |  | √ |  |  |  | 报告类型 1合并报表 2单季合并 3调整单季合并表 4调整合并报表 5调整前合并报表 6母公司报表 7母公司单季表 8 母公司调整单季表 9母公司调整表 10母公司调整前报表 11调整前合并报表 12母公司调整前报表 | 
 | 6 | comp_type | float | 12 |  |  |  | √ |  | 公司类型(1一般工商业2银行3保险4证券) | 
 | 7 | basic_eps | float | 12 |  |  |  | √ |  | 基本每股收益 | 
 | 8 | diluted_eps | float | 12 |  |  |  | √ |  | 稀释每股收益 | 
 | 9 | total_revenue | float | 12 |  |  |  | √ |  | 营业总收入 | 
 | 10 | revenue | float | 12 |  |  |  | √ |  | 营业收入 | 
 | 11 | int_income | float | 12 |  |  |  | √ |  | 利息收入 | 
 | 12 | prem_earned | float | 12 |  |  |  | √ |  | 已赚保费 | 
 | 13 | comm_income | float | 12 |  |  |  | √ |  | 手续费及佣金收入 | 
 | 14 | n_commis_income | float | 12 |  |  |  | √ |  | 手续费及佣金净收入 | 
 | 15 | n_oth_income | float | 12 |  |  |  | √ |  | 其他经营净收益 | 
 | 16 | n_oth_b_income | float | 12 |  |  |  | √ |  | 加:其他业务净收益 | 
 | 17 | prem_income | float | 12 |  |  |  | √ |  | 保险业务收入 | 
 | 18 | out_prem | float | 12 |  |  |  | √ |  | 减:分出保费 | 
 | 19 | une_prem_reser | float | 12 |  |  |  | √ |  | 提取未到期责任准备金 | 
 | 20 | reins_income | float | 12 |  |  |  | √ |  | 其中:分保费收入 | 
 | 21 | n_sec_tb_income | float | 12 |  |  |  | √ |  | 代理买卖证券业务净收入 | 
 | 22 | n_sec_uw_income | float | 12 |  |  |  | √ |  | 证券承销业务净收入 | 
 | 23 | n_asset_mg_income | float | 12 |  |  |  | √ |  | 受托客户资产管理业务净收入 | 
 | 24 | oth_b_income | float | 12 |  |  |  | √ |  | 其他业务收入 | 
 | 25 | fv_value_chg_gain | float | 12 |  |  |  | √ |  | 加:公允价值变动净收益 | 
 | 26 | invest_income | float | 12 |  |  |  | √ |  | 加:投资净收益 | 
 | 27 | ass_invest_income | float | 12 |  |  |  | √ |  | 其中:对联营企业和合营企业的投资收益 | 
 | 28 | forex_gain | float | 12 |  |  |  | √ |  | 加:汇兑净收益 | 
 | 29 | total_cogs | float | 12 |  |  |  | √ |  | 营业总成本 | 
 | 30 | oper_cost | float | 12 |  |  |  | √ |  | 减:营业成本 | 
 | 31 | int_exp | float | 12 |  |  |  | √ |  | 减:利息支出 | 
 | 32 | comm_exp | float | 12 |  |  |  | √ |  | 减:手续费及佣金支出 | 
 | 33 | biz_tax_surchg | float | 12 |  |  |  | √ |  | 减:营业税金及附加 | 
 | 34 | sell_exp | float | 12 |  |  |  | √ |  | 减:销售费用 | 
 | 35 | admin_exp | float | 12 |  |  |  | √ |  | 减:管理费用 | 
 | 36 | fin_exp | float | 12 |  |  |  | √ |  | 减:财务费用 | 
 | 37 | assets_impair_loss | float | 12 |  |  |  | √ |  | 减:资产减值损失 | 
 | 38 | prem_refund | float | 12 |  |  |  | √ |  | 退保金 | 
 | 39 | compens_payout | float | 12 |  |  |  | √ |  | 赔付总支出 | 
 | 40 | reser_insur_liab | float | 12 |  |  |  | √ |  | 提取保险责任准备金 | 
 | 41 | div_payt | float | 12 |  |  |  | √ |  | 保户红利支出 | 
 | 42 | reins_exp | float | 12 |  |  |  | √ |  | 分保费用 | 
 | 43 | oper_exp | float | 12 |  |  |  | √ |  | 营业支出 | 
 | 44 | compens_payout_refu | float | 12 |  |  |  | √ |  | 减:摊回赔付支出 | 
 | 45 | insur_reser_refu | float | 12 |  |  |  | √ |  | 减:摊回保险责任准备金 | 
 | 46 | reins_cost_refund | float | 12 |  |  |  | √ |  | 减:摊回分保费用 | 
 | 47 | other_bus_cost | float | 12 |  |  |  | √ |  | 其他业务成本 | 
 | 48 | operate_profit | float | 12 |  |  |  | √ |  | 营业利润 | 
 | 49 | non_oper_income | float | 12 |  |  |  | √ |  | 加:营业外收入 | 
 | 50 | non_oper_exp | float | 12 |  |  |  | √ |  | 减:营业外支出 | 
 | 51 | nca_disploss | float | 12 |  |  |  | √ |  | 其中:减:非流动资产处置净损失 | 
 | 52 | total_profit | float | 12 |  |  |  | √ |  | 利润总额 | 
 | 53 | income_tax | float | 12 |  |  |  | √ |  | 所得税费用 | 
 | 54 | n_income | float | 12 |  |  |  | √ |  | 净利润(含少数股东损益) | 
 | 55 | n_income_attr_p | float | 12 |  |  |  | √ |  | 净利润(不含少数股东损益) | 
 | 56 | minority_gain | float | 12 |  |  |  | √ |  | 少数股东损益 | 
 | 57 | oth_compr_income | float | 12 |  |  |  | √ |  | 其他综合收益 | 
 | 58 | t_compr_income | float | 12 |  |  |  | √ |  | 综合收益总额 | 
 | 59 | compr_inc_attr_p | float | 12 |  |  |  | √ |  | 归属于母公司(或股东)的综合收益总额 | 
 | 60 | compr_inc_attr_m_s | float | 12 |  |  |  | √ |  | 归属于少数股东的综合收益总额 | 
 | 61 | ebit | float | 12 |  |  |  | √ |  | 息税前利润 | 
 | 62 | ebitda | float | 12 |  |  |  | √ |  | 息税折旧摊销前利润 | 
 | 63 | insurance_exp | float | 12 |  |  |  | √ |  | 保险业务支出 | 
 | 64 | undist_profit | float | 12 |  |  |  | √ |  | 年初未分配利润 | 
 | 65 | distable_profit | float | 12 |  |  |  | √ |  | 可分配利润 | 
 | 66 | update_time | datetime |  |  |  |  | √ |  | 数据入库时间 | 

# 3_dws_web

## stock_daily_indicator 股票每日指标

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | date | date |  |  | √ |  |  |  | 日期 | 
 | 2 | code | varchar | 50 |  | √ |  |  |  | 股票代码 | 
 | 3 | capitalization | float | 12 |  |  |  | √ |  | 总股本（万股） | 
 | 4 | circulating_cap | float | 12 |  |  |  | √ |  | 流通股本（万股） | 
 | 5 | market_cap | float | 12 |  |  |  | √ |  | 总市值（亿元） | 
 | 6 | circulating_market_cap | float | 12 |  |  |  | √ |  | 流通市值（亿元） | 
 | 7 | return_1d | float | 12 |  |  |  | √ |  | 收益率—当天 | 
 | 8 | return_3d | float | 12 |  |  |  | √ |  | 收益率—近3天 | 
 | 9 | return_5d | float | 12 |  |  |  | √ |  | 收益率—近5天 | 
 | 10 | return_10d | float | 12 |  |  |  | √ |  | 收益率—近10天 | 
 | 11 | return_1m | float | 12 |  |  |  | √ |  | 收益率—近1个月 | 
 | 12 | return_3m | float | 12 |  |  |  | √ |  | 收益率—近3个月 | 
 | 13 | return_6m | float | 12 |  |  |  | √ |  | 收益率—近6个月 | 
 | 14 | return_1y | float | 12 |  |  |  | √ |  | 收益率—近1年 | 
 | 15 | return_3y | float | 12 |  |  |  | √ |  | 收益率—近3年 | 
 | 16 | money_1d | float | 12 |  |  |  | √ |  | 成交额—当天 | 
 | 17 | money_3d | float | 12 |  |  |  | √ |  | 成交额—近3天 | 
 | 18 | money_5d | float | 12 |  |  |  | √ |  | 成交额—近5天 | 
 | 19 | money_10d | float | 12 |  |  |  | √ |  | 成交额—近10天 | 
 | 20 | money_1m | float | 12 |  |  |  | √ |  | 成交额—近1个月 | 
 | 21 | money_3m | float | 12 |  |  |  | √ |  | 成交额—近3个月 | 
 | 22 | money_6m | float | 12 |  |  |  | √ |  | 成交额—近6个月 | 
 | 23 | money_1y | float | 12 |  |  |  | √ |  | 成交额—近1年 | 
 | 24 | money_3y | float | 12 |  |  |  | √ |  | 成交额—近3年 | 
 | 25 | turnover_rate_1d | float | 12 |  |  |  | √ |  | 换手率-当天 | 
 | 26 | turnover_rate_3d | float | 12 |  |  |  | √ |  | 换手率-近3天 | 
 | 27 | turnover_rate_5d | float | 12 |  |  |  | √ |  | 换手率-近5天 | 
 | 28 | turnover_rate_10d | float | 12 |  |  |  | √ |  | 换手率-近10天 | 
 | 29 | turnover_rate_1m | float | 12 |  |  |  | √ |  | 换手率—近1个月 | 
 | 30 | turnover_rate_3m | float | 12 |  |  |  | √ |  | 换手率—近3个月 | 
 | 31 | turnover_rate_6m | float | 12 |  |  |  | √ |  | 换手率—近6个月 | 
 | 32 | turnover_rate_1y | float | 12 |  |  |  | √ |  | 换手率—近1年 | 
 | 33 | turnover_rate_3y | float | 12 |  |  |  | √ |  | 换手率—近3年 | 
 | 34 | return_yearly_3d | float | 12 |  |  |  | √ |  | 年化收益率—近3天 | 
 | 35 | return_yearly_5d | float | 12 |  |  |  | √ |  | 年化收益率—近5天 | 
 | 36 | return_yearly_10d | float | 12 |  |  |  | √ |  | 年化收益率—近10天 | 
 | 37 | return_yearly_1m | float | 12 |  |  |  | √ |  | 年化收益率—近1个月 | 
 | 38 | return_yearly_3m | float | 12 |  |  |  | √ |  | 年化收益率—近3个月 | 
 | 39 | return_yearly_6m | float | 12 |  |  |  | √ |  | 年化收益率—近6个月 | 
 | 40 | return_yearly_1y | float | 12 |  |  |  | √ |  | 年化收益率—近1年 | 
 | 41 | return_yearly_3y | float | 12 |  |  |  | √ |  | 年化收益率—近3年 | 
 | 42 | maxdrawdown_3d | float | 12 |  |  |  | √ |  | 最大回撤—近3天 | 
 | 43 | maxdrawdown_5d | float | 12 |  |  |  | √ |  | 最大回撤—近5天 | 
 | 44 | maxdrawdown_10d | float | 12 |  |  |  | √ |  | 最大回撤—近10天 | 
 | 45 | maxdrawdown_1m | float | 12 |  |  |  | √ |  | 最大回撤—近1个月 | 
 | 46 | maxdrawdown_3m | float | 12 |  |  |  | √ |  | 最大回撤—近3个月 | 
 | 47 | maxdrawdown_6m | float | 12 |  |  |  | √ |  | 最大回撤—近6个月 | 
 | 48 | maxdrawdown_1y | float | 12 |  |  |  | √ |  | 最大回撤—近1年 | 
 | 49 | maxdrawdown_3y | float | 12 |  |  |  | √ |  | 最大回撤—近3年 | 
 | 50 | volatility_3d | float | 12 |  |  |  | √ |  | 波动率—近3天 | 
 | 51 | volatility_5d | float | 12 |  |  |  | √ |  | 波动率—近5天 | 
 | 52 | volatility_10d | float | 12 |  |  |  | √ |  | 波动率—近10天 | 
 | 53 | volatility_1m | float | 12 |  |  |  | √ |  | 波动率—近1个月 | 
 | 54 | volatility_3m | float | 12 |  |  |  | √ |  | 波动率—近3个月 | 
 | 55 | volatility_6m | float | 12 |  |  |  | √ |  | 波动率—近6个月 | 
 | 56 | volatility_1y | float | 12 |  |  |  | √ |  | 波动率—近1年 | 
 | 57 | volatility_3y | float | 12 |  |  |  | √ |  | 波动率—近3年 | 
 | 58 | riseday_3d | float | 12 |  |  |  | √ |  | 上涨天数占比—近3天 | 
 | 59 | riseday_5d | float | 12 |  |  |  | √ |  | 上涨天数占比—近5天 | 
 | 60 | riseday_10d | float | 12 |  |  |  | √ |  | 上涨天数占比—近10天 | 
 | 61 | riseday_1m | float | 12 |  |  |  | √ |  | 上涨天数占比—近1个月 | 
 | 62 | riseday_3m | float | 12 |  |  |  | √ |  | 上涨天数占比—近3个月 | 
 | 63 | riseday_6m | float | 12 |  |  |  | √ |  | 上涨天数占比—近6个月 | 
 | 64 | riseday_1y | float | 12 |  |  |  | √ |  | 上涨天数占比—近1年 | 
 | 65 | riseday_3y | float | 12 |  |  |  | √ |  | 上涨天数占比—近3年 | 
 | 66 | sharp_3d | float | 12 |  |  |  | √ |  | 夏普比率—近3天 | 
 | 67 | sharp_5d | float | 12 |  |  |  | √ |  | 夏普比率—近5天 | 
 | 68 | sharp_10d | float | 12 |  |  |  | √ |  | 夏普比率—近10天 | 
 | 69 | sharp_1m | float | 12 |  |  |  | √ |  | 夏普比率—近1个月 | 
 | 70 | sharp_3m | float | 12 |  |  |  | √ |  | 夏普比率—近3个月 | 
 | 71 | sharp_6m | float | 12 |  |  |  | √ |  | 夏普比率—近6个月 | 
 | 72 | sharp_1y | float | 12 |  |  |  | √ |  | 夏普比率—近1年 | 
 | 73 | sharp_3y | float | 12 |  |  |  | √ |  | 夏普比率—近3年 | 

## stock_daily_treemap 股票-行业-板块树状图数据

 | 序号 | 列名 | 数据类型 | 长度 | 小数位数 | 主键 | 自增 | 允许空 | 默认值 | 列说明 | 
 | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
 | 1 | date | date |  |  | √ |  |  |  | 日期 | 
 | 2 | code | varchar | 50 |  | √ |  |  |  | 股票代码 | 
 | 3 | ratio | float | 12 |  |  |  | √ |  | 收益率（%） | 
 | 4 | money | float | 12 |  |  |  | √ |  | 成交额（亿元） | 
 | 5 | display_name | varchar | 50 |  |  |  | √ |  | 中文名称 | 
 | 6 | s1name | varchar | 50 |  |  |  | √ |  | 申万行业1 | 
 | 7 | s2name | varchar | 50 |  |  |  | √ |  | 申万行业2 | 
 | 8 | s3name | varchar | 50 |  |  |  | √ |  | 申万行业3 | 
 | 9 | type | varchar | 50 |  |  |  | √ |  | 所属指数 | 

# 3_dws_stock_factor

# 3_dws_stock_label

