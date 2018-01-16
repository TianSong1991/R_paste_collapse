# R_paste_collapse
R语言group_by后进行聚组


 test4 <- test3 %>% group_by(公司名称) %>% 
          summarise(newstate = paste(部门状态,collapse = ","))
          
          
此处主要是group_by后进行paste的使用，使用collapse参数，就可以实现多行的聚组。此功能在left_join中去重特别好用。 
 
