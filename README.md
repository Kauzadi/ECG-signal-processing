# ECG-signal-processing
 ecg=LowPassFilter(ecg)
 ecg=HighPassFilter(ecg)
 ecg=Derivative(ecg)
 For i=1 to length(ecg)
 {
 ecg(i)=ecg(i)*ecg(i)
 }
 ecg=FiducialMark(ecg)
 For i=1 to length(ecg)
 {
 If(ecg(i)>Theshold)
 {
 Ecg(i)=ecg(i)
 }
 Else
 {
 Ecg(i)=0
 }
 }
 Return ecg
}
