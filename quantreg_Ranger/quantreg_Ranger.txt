# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Quantile regression with ranger Use quantregRanger With (In) R Software
install.packages("quantregRanger")
library("quantregRanger")
quantreg_Ranger = read.csv("https://raw.githubusercontent.com/timbulwidodostp/quantreg_Ranger/main/quantreg_Ranger/quantreg_Ranger.csv",sep = ";")
# Estimation Quantile regression with ranger Use quantregRanger With (In) R Software
quantregRanger = quantregRanger(y ~ ., data = quantreg_Ranger, params.ranger = list(mtry = 2))
quantregRanger
predict(quantregRanger, data = quantreg_Ranger[1:5, ], quantiles = c(0.1, 0.5, 0.9))
# Quantile regression with ranger Use quantregRanger With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished