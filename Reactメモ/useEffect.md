# userEffectの使い方

## Case1
```
  useEffect(()=>{
    console.log('useEffectが実行されました')
  })
```
→ コンポーネントが更新される度に実行される

## Case2
```
useEffect(()=>{
  console.log('useEffectが実行されました')
},[])
```
→ コンポーネントが初めて表示される時の一度だけ実行される

## CaseXX
```
useEffect(() => {
    console.log('useEffectが実行されました')

    return () => {
        console.log('コンポーネントがアンマウントしました')
    }
},[])
```
→ コンポーネントのアンマウント時に処理が実行される

## useLayoutEffectとは
→ useEffectとほぼ同じだが、<br>
useEffectは描画後に処理が実行されるのに対し、<br>
useLayoutEffectは描画前に処理が実行される。