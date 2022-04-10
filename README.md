# D-DayCount_Andriod
간단한 D-Day 카운터 어플.

4월 10일 study:

    주요내용:
        Calendar.getInstance()로 선언 -> set으로 초기화
        
        val today = GregorianCalendar()
        val year = today.get(Calendar.YEAR)
        val month = today.get(Calendar.MONTH)  //월은 0부터 시작하기때문에 실제 사용할때는 +1을해준다
        val day = today.get(Calendar.DATE)
        val dlg = DatePickerDialog(this, object : DatePickerDialog.OnDateSetListener {
                        override fun onDateSet(p0: DatePicker?, p1: Int, p2: Int, p3: Int) {
        		//세팅할 내용
                        }
                    }, year, month, day)
                    dlg.show()