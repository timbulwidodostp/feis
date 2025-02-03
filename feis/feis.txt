# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Estimating fixed effects individual slope models Use feis (feisr) With (In) R Software
install.packages("feisr")
library("feisr")
feis = read.csv("https://raw.githubusercontent.com/timbulwidodostp/feis/main/feis/feis.csv",sep = ";")
# (Estimation) Estimating fixed effects individual slope models Use feis (feisr) With (In) R Software
feis <- feis(Dependen ~ Independen_1 + Independen_2 + Independen_3 + as.factor(Factor) | Independen_4, data = feis, id = "Id")
summary(feis)
feistest <- feistest(feis, robust = TRUE, type = "all")
summary(feistest)
# Estimating fixed effects individual slope models Use feis (feisr) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished