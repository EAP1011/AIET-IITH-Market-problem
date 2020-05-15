import pandas as pd
import numpy as np
df=pd.read_csv("mixedData.csv",sep=(",|;"))
offices=df["TxnDate"].unique().tolist()
dates=df["taxAmt"].unique().tolist()
officesdet=[df.loc[df["TxnDate"]==x] for x in offices]
percentages=[(sum(officesdet[x]["vehicleclass"])/sum(officesdet[x]["invoiceamt"]))*100 for x in range(0,len(officesdet))]
print(percentages)
