# Советы по Laravel
Советы по Laravel
 [GitHub Pages](https://github.com/Saeedshoh/laravel-tips#test)
 * [Сгенерировать пароль во время создание пользователя](#set_password)



<a name="set_password"></a> 
######Сгенерировать пароль во время создание пользователя
    public function setPasswordAttribute($password)
    {
        if($password != null) {
            $this->attributes['password'] = bcrypt($password);
        }
    }
    
    
    
    
    
