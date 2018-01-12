# ZXSDatePickerView
日期选择控件的简单封装

调用方式：
(1)初始化 [[ZXSDatePicterView alloc] init]
(2)调用方法 
[self.datePickerView showDatePickerBirthdayWithDate:[NSDate date] minDate:nil maxDate:nil block:^(NSDate *selectDate) {
        NSDateFormatter *formatter = [[NSDateFormatter alloc] init];
        [formatter setDateFormat:@"yyyy-MM-dd"];
        _dateLabel.text = [formatter stringFromDate:selectDate];
    }];
    
    
    需要导入 Masonry布局
