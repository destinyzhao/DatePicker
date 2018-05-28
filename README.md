# DatePicker
Custom DatePicker

```
//年-月-日-时-分
JXDatePickerView *datepicker = [[JXDatePickerView alloc] initWithDateStyle:DateStyleShowYearMonthDayHourMinute CompleteBlock:^(NSDate *selectDate) {
                
  NSString *dateString = [selectDate stringWithFormat:@"yyyy-MM-dd HH:mm"];
  NSLog(@"选择的日期：%@",dateString);
  [btn setTitle:dateString forState:UIControlStateNormal];
}];
datepicker.dateLabelColor = [UIColor orangeColor];//年-月-日-时-分 颜色
datepicker.datePickerColor = [UIColor blackColor];//滚轮日期颜色
[datepicker show];
```
