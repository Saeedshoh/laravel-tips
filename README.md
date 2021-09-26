# Советы по Laravel
Советы по Laravel



    public function setPasswordAttribute($password)
    {
        if($password != null) {
            $this->attributes['password'] = bcrypt($password);
        }
    }
